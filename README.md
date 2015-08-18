# Server

```objective-c
[Database 설정]
/Applications/apache-tomcat-8.0.24/conf/web.xml 수정

    <servlet>
        <servlet-name>jsp</servlet-name>
        <servlet-class>org.apache.jasper.servlet.JspServlet</servlet-class>
        <init-param>
            <param-name>fork</param-name>
            <param-value>false</param-value>
        </init-param>
        <init-param>
            <param-name>xpoweredBy</param-name>
            <param-value>false</param-value>
        </init-param>
        <init-param>
            <param-name>dbConnection</param-name>
            <param-value>jdbc:mysql://localhost:3306/pfxstudio</param-value>
        </init-param>
        <init-param>
            <param-name>dbUnicode</param-name>
            <param-value>?useUnicode=true</param-value>
        </init-param>
        <init-param>
            <param-name>dbCharacterEncoding</param-name>
            <param-value>characterEncoding=UTF-8</param-value>
        </init-param>
        <init-param>
            <param-name>dbUser</param-name>
            <param-value>pfxstudio</param-value>
        </init-param>
        <init-param>
            <param-name>dbPassword</param-name>
            <param-value>xxxxxxxxxx</param-value>
        </init-param>
        <load-on-startup>3</load-on-startup>
    </servlet>


[lib Copy]
/Users/pfxstudio/Documents/Server.checkout/trunk/Server/WebContent/WEB-INF/lib
jar 파일 복사
MySQL 접속에 필요한 mysql-connector-java-5.1.31-bin.jar 있나 확인

[Eclipse 설정]
Eclipse 설정에 Server - Runtime Environments - Add Tomcat

[Server 프로젝트 설정]
Project Facets - Runtimes - Tomcat 선택
Java Build Path - Library - JRE System Library 삭제 후 재 등록
```


#Customization


# PFXStudio

Mobile : http://pfxstudio.modoo.at/

Twitter : http://twitter.com/pfxstudio

Facebook : http://facebook.com/pfxstudio

iOS AppStore : https://itunes.apple.com/us/artist/ppark/id448017898

Google Play : https://play.google.com/store/apps/developer?id=PFXStudio


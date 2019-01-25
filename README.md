# SpringBoot-Test
SpringBoot快速入门
springBoot 精髓 SpringBoot不是对Spring功能上的增强，而是提供了一种快速使用Spring的方式
	                如果使用springboot必须使用maven或者gradle
                起步依赖：
                    一个框架的jar包配置的集合。
                自动配置：
                    默认对框架进行整合，约定大于配置。
      
      ---pom
                    
 <!--添加springBoot启动器-->
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>2.0.2.RELEASE</version>
    </parent>
    <!--指定jdk版本-->
    <properties>
        <java.version>1.8</java.version>
    </properties>
    <!--web测试工程,需要使用springMVC引入web相关-->
    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
            //不需要指定版本号  父类启动器spring-boot-starter-parent的顶级父类有一个 dependencyManagement  锁定了版本,一切dependencyManagement为准
          
          
        </dependency>
    </dependencies>

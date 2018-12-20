# spring-boot-swagger-starter
spring-boot-swagger-starter


使用：
1、
        <dependency>
            <groupId>cendy.chen.org</groupId>
            <artifactId>swagger-starter</artifactId>
            <version>0.0.1</version>
        </dependency>
       
2、
各个Action增加swagger注解
a、@Api(value = "短信相关信息") 在Controller类上注解，说明这个Controller作用

b、@ApiOperation(value = "查询短信剩余条数",response=ResultMap.class) 在controller方法上注解，说明这个方法的作用

c、@ApiParam(required = true,value = "实体id")@RequestParam 在controller方法的参数上注解，说明这个字段       


3、applicaiton.yml
swagger:
  groupName: xxxx
  title: xxxx
  description: xxx
  termsOfServiceUrl:
  version: 1.0
  contactName: xx
  contactUrl:
  contactEmail: xx@xx.com
  paths: /xx.*, /xx.*
  license:
  licenseUrl:
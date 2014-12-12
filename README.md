jea框架集成的样例项目<br>
各分层的简易说明：<br>
1、web层，允许单独部署，可通过springMVC、REST、SOAP提供web服务<br>
2、bridge层，为Web层提供远程调用服务，作为WebServer与APPServer之间的桥梁<br>
3、facade层，封装实际业务逻辑，DB事务由它控制<br>
4、service层，封装业务原子逻辑，通过调用dao层或integration层实现<br>
5、dao层，封装与DB的操作<br>
6、integration层，封装与外部系统的连接操作<br>
7、common层，公共层，当Web层独立部署时，common层可放置WebServer与AppServer都要使用的配置文件和Bean类<br>

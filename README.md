### Ŀ¼����
* config-resources:Զ��������ԴĿ¼
* config-server-git:�ֲ�ʽ��������
* eureka-client:eureka�ṩ�߷���
* eureka-consumer:eureka�����߷���
* eureka-server:eureka����ע������
* hystrix-dashboard�����Hystrixָ�����ݵĿ��ӻ����
* turbine:�ۺϸ߿��ö�ʵ�������Hystrix����ָ������,��hystrix-dashboard���

��Ŀ����˳��eureka-server>config-server-git>eureka-client>eureka-consumer>turbine>hystrix-dashboard
### spring cloudѧϰ�ܽ�
1. ribbon��eureka�ͻ��˸��ؾ��⣬�ڷ������Ѷ�ʹ��,nginx��������ؾ��⣬������ǰ�˷��������ʸ��ؾ���

2. application.yml�ɸ���bootstrap.yml�ڳ�Զ������������ԣ�����Զ��������Ҫ����`spring.cloud.config.allowOverride=true`

3. Spring Cloud Config���ܽ���ʱע�⣺JCE�汾��Unlimited Strength Java Cryptography Extension��Ҫ�����л���jdk�汾ƥ��

4. ������⣺����ע�ᵽeurekaע�����ĵĶ��Ƿ��񣬷����(�����ṩ��)���ͻ���(����������)��Щ�Ǹ�����Ŀ��ƾ�����

5. ���ע�������ж�̨`spring.application.name`��ͬ�ķ���������ʱ�ͻᴥ�����ؾ������(�����ø��ؾ�����ʷ�ʽ)
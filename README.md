### Ŀ¼����
* api-gateway:��������
* config-resources:Զ��������ԴĿ¼
* config-server-git:�ֲ�ʽ��������
* eureka-client:eureka�ṩ�߷���
* eureka-consumer:eureka�����߷���
* eureka-server:eureka����ע������
* hystrix-dashboard�����Hystrixָ�����ݵĿ��ӻ����
* turbine:�ۺϸ߿��ö�ʵ�������Hystrix����ָ������,��hystrix-dashboard���

��Ŀ����˳��eureka-server>config-server-git>eureka-client>eureka-consumer>api-gateway|(turbine>hystrix-dashboard)
### spring cloudѧϰ�ܽ�
1. spring cloud�ĸ��ؾ������������ע�����ĵķ����ĵ���,nginx��zuul�����ڶ���ͻ��˷���ĸ��ؾ���

2. application.yml�ɸ���bootstrap.yml�ڳ�Զ������������ԣ�����Զ��������Ҫ����`spring.cloud.config.allowOverride=true`

3. Spring Cloud Config���ܽ���ʱע�⣺JCE�汾��Unlimited Strength Java Cryptography Extension��Ҫ�����л���jdk�汾ƥ��

4. ������⣺����ע�ᵽeurekaע�����ĵĶ��Ƿ��񣬷����(�����ṩ��)���ͻ���(����������)��Щ�Ǹ�����Ŀ��ƾ�����

5. zuul���صĸ߿��ã�Ŀǰû�ҵ�zuul��ص�����nginx+Keepalived�����Ĺ���ת�Ʒ�������������nginx��Ϊ�������->ʹ��nginx�һ�����⿪�ŵĿͻ��˷���Ⱥʹ��Keepalived������ת�ƣ��һ��zuul��Ⱥ�����ؾ���·���ڲ�����ʹ��nginx�ĸ��ؾ�����Ʒ������zuul��Ⱥ

6. eureka-serverע�����ĸ߿��þ��ǲ���һ�����Ƽ�Ⱥ������ע�ᣬ���ิ��

7. ��Ⱥ��������ע��ʱ������ֻע�������һ��Ȼ�����ü�Ⱥ�ĸ������Ը��Ƹ�����ע�����ģ�ԭ�������ֻע���һ̨������̨ע�����Ĺ��ˣ�������������޷�ע�ᵽ��Ⱥ�����ˣ�������Ȱѹ��˵�ע����������

8. ��������ע������2̨��Ⱥ��3̨��Ⱥ��û�о��в�ͬ������Ϊʲô����˵3̨��Ⱥ����߿����Լ�Ⱥ
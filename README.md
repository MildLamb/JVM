# JVM
## JVM 体系结构
![image](https://user-images.githubusercontent.com/92672384/158717980-7432027f-eefd-42e3-820d-f2bde3164683.png)

## 类加载器和双亲委派机制
![{{}FV6ZC{QX3L_JSX 610F4](https://user-images.githubusercontent.com/92672384/158719714-80892a29-8811-43be-a4fc-58994cd219eb.png)

![image](https://user-images.githubusercontent.com/92672384/158723202-bc487064-cda1-42fd-a2b3-b980907e6a95.png)

- 双亲委派：双亲委派机制时JVM类加载的默认使用的机制，其原理是:当一个类加载器收到类加载任务时，会先交给自己的父加载器去完成，因此最终加载任务都会传递到最顶层的BootstrapClassLoader，只有当父加载器无法完成加载任务时，才会按照由父级到子集的顺序尝试自己来加载。

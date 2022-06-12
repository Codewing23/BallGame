
# 技术栈

![在这里插入图片描述](https://img-blog.csdnimg.cn/cec7ed6eb0244f4bac5b24e0a9d58d1b.png)


# 开发准备


- 开发环境：jdk1.7+
- 开发工具：IDEA、 Eclipse


# 开发过程

## 显示画框

```java
public class Game extends JPanel {
    private final static int WIDTH = 1024;
    private final static int HEIGHT = 567;
    public static void main(String[] args) {
        // 创建画框对象
        JFrame jFrame = new JFrame("小球大作战");
        // 创建画布对象【向上造型】
        JPanel jPanel = new Game();
        // 将画布添加到画框中
        jFrame.add(jPanel);
        // 将画框展示出来
        jFrame.setVisible(true);
        // 设置画框大小
        jFrame.setSize(WIDTH, HEIGHT);
        // 相对位置，相对于上下左右都是等长的，即将画框放在屏幕中央
        jFrame.setLocationRelativeTo(null);
        // 窗体默认关闭方式
        jFrame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        // 设置画框的优先级，使其总是显示在最上方
        jFrame.setAlwaysOnTop(true);
    }
}
```

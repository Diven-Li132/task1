任务1：
按顺序打印出APP，ViewController 生命周期的各个事件

1.App 生命周期的各个事件：
点击程序图标->执行main函数->通过UIApplicationMain函数->初始化UIApplication对象并且为它设置代理对象->UIApplication对象->程序退出结束
代理对象的部分设置如下：

程序载入后->applicationDidFinishLaunching

将要进入非活动状态->applicationWillResignActive

程序进入活动状态->applicationDidBecomeActive

程序进入后台->applicationDidEnterBackground

程序从后台将要重新进入前台->applicationWillEnterForeground

内存警告，程序将要终止->applicationDidReceivememoryWarning

程序将要退出结束->applicationWillTerminate

2.UIViewController 生命周期的各个事件：
alloc/init->loadView->viewDidload->viewWillAppear->viewDidAppear->viewWillDisappear->viewDidDisappear->dealloc

任务2：
写出五种常用的UI控件

 UIViewController（页面）
 UIView（通用视图）
 UIImageView（图片视图）
 UILabel（文本）
 UIButton（按钮）
![image](https://user-images.githubusercontent.com/109218561/178728944-0d61afd3-77cf-4581-bca5-a4414fafc2d2.png)


任务3：
列举出三个 UITableViewDelegate 声明的方法

//1.选中某行cell调用此方法
-(void)tableView:(UITableView *)tableView didSelectRowAtIndexPath:(NSIndexPath *)indexPath;
//2.自定义每组头部的view
-(UIView *)tableView:(UITableView *)tableView viewForHeaderInSection:(NSInteger)section; 
//3.自定义每组尾部的view
-(UIView *)tableView:(UITableView *)tableView viewForFooterInSection:(NSInteger)section;

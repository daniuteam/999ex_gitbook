# Raydium CPMM加池子教程

CPMM是Raydium最新推出的一个流动性产品，具有以下特点：

* **新的做市逻辑：**&#x91C7;用了新的 CPMM 做市模式，有别于之前V2的AMM
* **不需要市场ID：**&#x43;PMM不再需要Openbook市场ID，可省去一笔ID创建费用
* **创池成本更低：**&#x43;PMM的池子创建收费0.2sol，是原先AMM池子的一半
* **支持度不够：**&#x4F8B;如PEPE机器人等尚不支持CPMM版本，只有我们的市值机器人支持
* **交易问题 ：**&#x52A0;了CPMM池子之后，偶尔可能会遇到无法交易的问题

### 1、加池子

我们打开Raydium的官网：<https://raydium.io/liquidity-pools/>，点击右边的`创建`按钮

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F6WDax2cGwL3nfF3tT2YM%2F%E5%88%9B%E5%BB%BA%E6%B1%A0.png?alt=media&#x26;token=6b0b3519-3781-464c-845b-476924b2a0e8" alt=""><figcaption></figcaption></figure>

打开之后，选择**标准AMM池**，然后继续下一步

* 集中池创建麻烦，且价格不能波动太大，所以一般我们推荐创建标准AMM池

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F5k4P6N0Sl51S4e092l8l%2F%E6%A0%87%E5%87%86AMM%E6%B1%A0.png?alt=media&#x26;token=e69cc612-9a56-439a-ad75-8f0616d40008" alt=""><figcaption></figcaption></figure>

### 2、确定价格和比例

在新的页面，我们需要填写相应的代币与数量，进行流动性创建

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F6KnkbCStHVgrr3mZew4B%2F%E4%BB%A3%E5%B8%81%E6%95%B0%E9%87%8F%E4%B8%8Esol%E6%95%B0%E9%87%8F.png?alt=media&#x26;token=da6f30d7-f139-4fee-8cce-d9800dfbe7f0" alt=""><figcaption></figcaption></figure>

* **代币数量：**&#x4F60;要添加到池子里面的代币数量（你发行的代币）
* **Sol数量：**&#x4F60;的交易对代币（报价代币）
* **开盘时间：**&#x4EE3;币开始交易的时间。这个时间之前，池子无法交易（UTC时间，与北京时间有8个小时时差）
* **开盘价格：**&#x4E5F;就是代币初始价格，取决于你的代币数量与Sol数量。例如，我初始放入1亿枚代币和1个sol进入池子，那么我的开盘价格就是：0.00000001sol，换算成USDT就是0.00000182U

例如我填好的，类似于下面这样：

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F9pAHjRwBs3WTNzWpkWTV%2F%E5%BC%80%E7%9B%98%E6%97%B6%E9%97%B4.png?alt=media&#x26;token=4277bae9-bc6b-4cab-86e8-14e5d67055fa" alt=""><figcaption></figcaption></figure>

关于开盘时间这一块，在设置的时候，Raydium很人性化的给予了自动转换时区的功能，UTC时间与北京时间自动转换，所以设置起来就比较方便了，例如下面这样

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F3xlE48Jt5OR19IP11nyY%2F%E6%97%B6%E9%97%B4%E8%AE%BE%E7%BD%AE.png?alt=media&#x26;token=a5b2a29f-5996-42cb-b848-962a30f3ef03" alt=""><figcaption></figcaption></figure>

确定好没问题之后，点击初始化流动性，钱包确认支付费用就可以了。（注：加池手续费大概0.2sol左右）

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FBrFiZays0USC6APTy5NE%2Fsol%E9%92%B1%E5%8C%85%E7%A1%AE%E8%AE%A4.png?alt=media&#x26;token=5f5b599b-8250-4b7c-a5da-1c4acf454417" alt=""><figcaption></figcaption></figure>

池子创建成功后，会有个提示给你，如下图所示

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FftiqeDrAALn7p53AUnb4%2F%E6%B1%A0%E5%AD%90%E5%88%9B%E5%BB%BA%E6%88%90%E5%8A%9F.png?alt=media&#x26;token=342670d1-a14a-46f4-9ce2-41c4adb5620c" alt=""><figcaption></figcaption></figure>

### 4、撤池子

池子加好之后怎么撤呢？这里也和大家说一下

我们打开Raydium，找到`我的投资组合`，页面链接：<https://raydium.io/portfolio/> 选择标准流动池，就能看到自己的池子了

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FpcHa3LHnubNQKBpzRgzg%2F%E6%92%A4%E6%B1%A0%E5%AD%90%E6%8C%89%E9%92%AE.png?alt=media&#x26;token=79e5476c-11ef-4f40-95b0-71a837740cb6" alt=""><figcaption></figcaption></figure>

* 注：如果你设置了开盘时间，那要等到开盘后，才能看到池子

此时，如果你想撤池子，选择那个“-”按钮就可以了，如下所示：

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FeDxvdect4BFgWgf0iIXs%2F%E6%92%A4%E6%B1%A0%E5%AD%90%E6%AF%94%E4%BE%8B.png?alt=media&#x26;token=c2319054-5152-424a-859e-75d252f1d6df" alt=""><figcaption></figcaption></figure>

选择你要撤池子的比例，点击`移除流动性`，然后钱包确认，就可以了

### 5、相关问题

**1）**&#x43;PMM**有什么优点/缺点？**

* 答：CPMM的优点就是不用创建市场ID，省了笔钱。缺点就是一些狙击机器人不支持V3，没法用

**2）加了**CPMM**池子后能`锁池`吗？**

* 答：同样可以烧池子

**3）代币没有关闭冻结权限，怎么办？**

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FwBe30g7Vb7UHSnTXqtqj%2F%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20240528170459.png?alt=media&#x26;token=d2570cbb-cc7f-4d56-b625-bc16c48a5014" alt=""><figcaption></figcaption></figure>

* 答：需要去权限管理工具那里关闭冻结权限：<https://solana.999ex.io/control>，方可继续操作。如果还是有提示，可能是raydium有缓存，需要更换网络或者刷新重试

**4）“应用程序错误：发生了客户端异常”应该怎么解决**

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F4qFu0DrwwkUGePeN74qq%2F%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20241001101529.png?alt=media&#x26;token=d547b151-9262-4afd-9573-153c9ab7f47e" alt=""><figcaption></figcaption></figure>

* 答：出现这个问题的原因主要是在谷歌浏览器开启翻译导致的，只要将翻译关闭，重新刷新试一下，这个问题就不会出现了

以上就是关于Raydium CPMM加池子/撤池子的全部教程了，如果有任何问题，请进入我们的电报群：<https://t.me/tool999ex>，找志愿者解答，谢谢

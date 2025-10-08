# PumpFun一键捆绑卖出教程

### 怎么理解PumpFun一键捆绑卖出这个功能？

我们假设这样一种情况，当你使用PUMP捆绑买入功能在多个地址内买入代币，或者拉盘刷量期间操作多个地址买入代币后，想将这些地址里面的代币全部卖出，应该怎么办？

传统的方式就是三种：

* **第一种：**&#x624B;动卖。不断地切换钱包操作。这样不仅慢，而且机器人会泡在你的前面，不合适
* **第二种：**&#x673A;器人卖。通过我们的机器人可以自动化卖出，省去了手动操作的麻烦，但是速度跟不上
* **第三种：**&#x5F52;集后卖。将代币归集到一个地址后统一卖出。听起来比较合适，但也是麻烦，多了一步归集的操作

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FbDgCYoCEDBMjAFi6aSsC%2FPUMP%E6%8D%86%E7%BB%91%E5%8D%96%E5%87%BA.jpg?alt=media&#x26;token=125a0cc4-f200-482c-b97a-e8bdfe275e56" alt=""><figcaption></figcaption></figure>

基于此，我们开发了一键捆绑卖出的功能，导入钱包私钥后，即可**一次性将所有钱包内的相关代币全部卖出。**&#x76EE;前一次最多支持15个地址，如果钱包比较多，可以多导入几次。

### PUMP一键捆绑卖出教程

#### 1、配置卖出参数

我们打开999ex.io Tool的一键卖出工具：<https://solana.999ex.io/sellpump> ，或者在官网导航栏找到捆绑卖出的按钮

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F0e5Do2qKWFjFvpPmIawl%2F1-%E6%8D%86%E7%BB%91%E5%8D%96%E5%87%BA.png?alt=media&#x26;token=0f31af3e-37d6-4531-a38e-24be72a9341b" alt=""><figcaption></figcaption></figure>

进入到捆绑卖出页面后，我们填写相关的参数

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2Fgigz1W2U0msc8BQRPp9M%2F5-%E5%8D%96%E5%87%BA%E5%8F%82%E6%95%B0.png?alt=media&#x26;token=99d33768-2bbc-4398-a08c-eb35e54b1d76" alt=""><figcaption></figcaption></figure>

* **pump代币：**&#x8F93;入pump代币合约地址，点击查询
* **代币名称：**&#x67E5;询后自动识别，无需填写
* **代币简称：**&#x67E5;询后自动识别，无需填写
* **Jito捆绑小费：**&#x9ED8;认是0.001sol。如果捆绑失败，可尝试提高Jito小费（4个地址以内不需要，4个地址以上需要）
* **捆绑钱包设置：**&#x8BF7;注意,链接钱包不参与捆绑卖出,所有费用由第一个导入的地址支付!

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FbpglD1pYk6zaiW7S9kFP%2F6-%E5%AF%BC%E5%85%A5%E7%A7%81%E9%92%A5.png?alt=media&#x26;token=c40d0765-79d2-4a59-9a2f-a7e907b2496d" alt=""><figcaption></figcaption></figure>

导入钱包后，我们点击刷新余额，大概就是这样一个页面

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F1BJrZ7L7JpNDXIRmCZO9%2F7-%E5%8D%96%E5%87%BA%E9%85%8D%E7%BD%AE.png?alt=media&#x26;token=f813cbf6-1a72-4aa6-bfd8-912755188e50" alt=""><figcaption></figcaption></figure>

从这张截图中我们发现一个问题：第一个钱包尾号为wnnt的地址，钱包内的Sol余额比较少（必须大于0.3个sol），无法支付卖出费用。

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FxFzE8FSs5a9TjWVASLZh%2F8-%E5%AF%B9%E8%B0%83%E4%BD%8D%E7%BD%AE.png?alt=media&#x26;token=63227f06-4d7f-4039-b9bc-ff34c27e1373" alt=""><figcaption></figcaption></figure>

因此，我们需要转一些sol给第一个钱包地址

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FQyOHaL8AOXPoq9H8ZnUr%2F8-2%E4%BD%99%E9%A2%9D%E5%A4%9F%E4%BA%86.png?alt=media&#x26;token=8f3e6d47-8f77-40b2-95e9-fa203e5bbbe0" alt=""><figcaption></figcaption></figure>

搞定后，在确认其他地方也没有问题后，我们点击立即卖出

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FoRjd9JwnszKBKiRphKgp%2F9-%E7%AB%8B%E5%8D%B3%E5%8D%96%E5%87%BA.png?alt=media&#x26;token=60c5621e-db1f-4ad3-9376-06f0f54adb25" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
☝当仅导入四个地址时, 无需 使用Jito捆绑功能,成功率较高,推荐使用!

☝最多支持15个地址捆绑卖出,当超过四个地址时,需要使用 Jito的捆绑功能。

☝由于网络环境、Jito节点等复杂影响,该功能可能出现失败。尽快确认。

☝为提高成功率,在弹出钱包后,请尽快确认。

☝若捆绑失败,无任何费用,请尝试更换RPC节点,并考虑在链上活跃度较低的时段再次尝试。
{% endhint %}

#### 2、确定钱包卖出

当我们点击**立即卖出，**&#x5E73;台的前端会自动执行，将地址内的代币全部卖出。注意，是全部卖出，不可以指定数量哦

等待15\~30秒，如果还没有成功，大概率就是失败了，需要重新提交。

如果卖出成功，会出现以下提示

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2Fl0qIiVkC1EtII20e8kM3%2F11-%E5%8D%96%E5%87%BA%E6%88%90%E5%8A%9F.png?alt=media&#x26;token=f4adff65-333e-4758-b381-46ddbd320aee" alt=""><figcaption></figcaption></figure>

之后我们点击刷新余额，就能看到余额为0了

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FVrYIE3AdZCQdwwJH7ZCT%2F12-%E5%88%B7%E6%96%B0%E4%BD%99%E9%A2%9D.png?alt=media&#x26;token=1788f66b-ad6d-48c3-9340-ed0f2cb3ebdf" alt=""><figcaption></figcaption></figure>

### 疑问解答

1. **一键捆绑卖出需要收费吗？**
   * **答：**&#x6BCF;个地址收费0.01sol，这部分费用全部由第一个钱包出
2. **一键捆绑卖出是卖出钱包内的所有代币吗？**
   * **答：**&#x6346;绑卖出是卖出你选择的那个PUMP的币，没有选择的币是不受影响的
3. **卖出失败是怎么回事？**
   * **答：**&#x6B63;常4个地址以内，应该不会失败。超过4个地址之后，需要用Jito捆绑。捆绑的话可能会失败，这个时候需要刷新后重试，并增加Jito费用

如何您还有其他问题，都可以进入Telegram电报群找志愿者解答： <https://t.me/tool999ex>

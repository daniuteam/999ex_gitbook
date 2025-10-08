# Solana销毁代币、烧池教程

* **烧池子：**&#x5C06;LP代币销毁，无法撤出流动性
* **燃烧代币：**&#x5C06;任何代币销毁，减少代币供应量

### 烧池概念问答

**1、LP是什么东西？**

* 答：LP本身也是一个代币。当您在创建流动性的时候，Raydium会给你发放一些LP代币作为凭证（类似于：银行存单）。以后你去撤池子，钱包就会自动将LP转给Raydium销毁掉，然后Raydium就让你把流动性撤出。所以，它是一个流动性/池子凭证。

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2F3FoW68yyXZZEMJwnUrLG%2FLp.png?alt=media&#x26;token=4d4eeae5-43e1-4808-80f8-ddbfe25ed50a" alt=""><figcaption></figcaption></figure>

**2、销毁LP又是什么意思？**

* 答：前面我们提到，LP是一个流动性凭证。Raydium只认Lp，不认钱包（*银行只认存单，不认人*）。如果将Lp转移给被人，那么别人就可以撤。谁有这个LP，谁能撤池子。如果将LP销毁掉，那就说明这个LP不存在了，无法再撤出流动性了。这个就是我们说的**烧池子**。

**3、烧池子是什么意思？池子烧完还能交易吗？**

* 答：很多人误区，认为池子烧了，池子里面的Sol和代币就不存在了，这是错误的观念。销毁LP=烧池子=无法撤池子。注意，池子依然存在，只是不能撤了而已。所以，**烧完池子后还能交易**，不受影响。
* 如果你自己将银行存单烧了，这个笔钱还是在银行的，只能没人可以取了。

通过我们的工具，大家不仅可以烧池子，也能将代币销毁掉，具体操作的教程如下：

打开链接<https://solana.999ex.io/burn>，右上角连接你的Phantom钱包（如未安装钱包，可参考→[Phantom安装教程](https://help.999ex.io/sol/phantom)）

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FKw1dQjuslFX4hwVazhIQ%2F%E9%80%89%E6%8B%A9%E9%92%B1%E5%8C%85.png?alt=media&#x26;token=80530c3a-becd-45dc-85bd-654844608863" alt=""><figcaption></figcaption></figure>

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FqrmzAYWhaxYQK0PAPaYF%2F%E9%80%89%E6%8B%A9phantom.png?alt=media&#x26;token=d0611d81-9cfd-4165-b7c4-f1dafc5a02bd" alt=""><figcaption></figcaption></figure>

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FOY5Y97N5BOzV99Hh17SO%2F%E9%92%B1%E5%8C%85%E5%B7%B2%E8%BF%9E%E6%8E%A5.png?alt=media&#x26;token=04d64a8e-bcdb-4909-9fa1-f32a10d72207" alt=""><figcaption></figcaption></figure>

连上钱包后，在选择框能看到你钱包内目前拥有的代币和LP

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FGw3O9z71kzUgfKPuS9Qr%2F%E7%87%83%E7%83%A7%E4%BB%A3%E5%B8%81%E9%A1%B5%E9%9D%A2.png?alt=media&#x26;token=53265ef8-fc43-4d2b-9206-35d3b1ebde09" alt=""><figcaption></figcaption></figure>

这个时候，你想烧毁代币，就点击代币，大概页面是这样的：

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FxwL2xhUItWZqAGobKsyB%2F%E7%83%A7%E6%AF%81%E4%BB%A3%E5%B8%81.png?alt=media&#x26;token=99033709-e524-495c-9603-7072cec04d3e" alt=""><figcaption></figcaption></figure>

想烧毁LP，就点击LP。烧毁LP，就是烧池子，大概页面是这样的

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FjIpMpGfInIX1F58o0W1C%2F%E9%94%80%E6%AF%81LP.png?alt=media&#x26;token=b2a8a7c1-77ea-41e7-8ca1-1318a94a83c8" alt=""><figcaption></figcaption></figure>

当查询到你钱包的LP数量之后，你可以填入销毁LP的数量，然后点击“销毁”就行。当然，你想全部销毁，就把右边那个“全部销毁并关闭账户”给勾选上，然后点击销毁，钱包确认就行了

<figure><img src="https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FJRG2vFoAzHYppobwn8zv%2F%E9%94%80%E6%AF%81%E5%B9%B6%E5%85%B3%E9%97%AD%E8%B4%A6%E6%88%B7.png?alt=media&#x26;token=5e3708ba-7c55-4d97-a251-731c2ad81135" alt=""><figcaption></figcaption></figure>

## 疑问解答

#### 1、关闭账户是什么意思？

* **答：**&#x4F60;每收到一个新的代币，Solana系统会自动在你的地址里开设一个代币存储账户。所谓“关闭账户”，就是把代币全部销毁，账户也关掉的意思。关闭账户并不影响你自己的钱包，因此不用担心。

**2、NFT可以销毁吗？**

* **答：**&#x5728;Orca加池子获得是NFT，这个暂时是不支持销毁/烧池的。目前可以销毁的是Ryadium和Meteora的LP。

**3、烧池后还能撤回流动性吗？**

* **答：**&#x70E7;池后，永久无法撤出流动性

有任何烧池子的问题，可以在电报群联系志愿者：<https://t.me/tool999ex>

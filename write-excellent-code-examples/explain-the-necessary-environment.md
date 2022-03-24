# 解释必要的环境

你要避免让人们对你的代码感到兴奋，然后无法在他们自己的环境中工作。你可以通过几种方式来解决这个问题：

-   **编写防御性的代码**：在试图访问它们之前检查依赖性。
-   **检查在线和HTTP状态**：如果你的代码需要从网络服务中提取数据，就说用户需要在线才能运行它。例如，我有过很多抱怨，说我的一些JavaScript例子在离线或不运行本地服务器的情况下不能工作。很明显，我没有解释它需要实时数据，而且出于安全考虑，JavaScript的某些功能只有在通过HTTPS访问时才能使用，而不是在文件系统上。
-   **列出需要的东西**：说说你的依赖性是什么。例如："需要Node和NPM"或 "在Microsoft Edge 85和更新的版本中运行"。如果需要第三方的依赖，为你的读者找到一个好的教程来安装它们，并将依赖的名称链接到它。
-   **提供一个简单的测试脚本**：检查正确的设置（例子见 [test file for GeoMaker](http://github.com/codepo8/GeoMaker/blob/3d88e693698965b802539d2a467e05f1f67cff76/test.php)）。
-   **为演示提供一个开发者密钥**：但要明确告诉人们，要实现你的代码，他们需要一个自己的密钥。提供一个申请密钥的链接。

你无法预测人们在执行你的代码时可能做错的所有事情，但这些是防止挫折的好方法。这使我想到了代码示例的一个重要部分：允许复制和粘贴。
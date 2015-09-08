# WBInAppHelper
Easy in-apps for your applications

# Installation
1) Copy files to your project
2) Call, when you have list of your product ids:
```obj-c
[WBInAppHelper setProductsList:@[@"com.my.product"]];
```
3) Get price of product:
```obj-c
NSString *str = [WBInAppHelper priceStringFromProductId:@"com.my.product"];
```
4) Call:
```obj-c
[WBInAppHelper payProduct:@"com.my.product" resBlock:^(BOOL success, NSError *err){
    if (success) {
        //paid successfully
    }
}];
```
5) Check is product paid anywhere in your app:
```obj-c
BOOL paidProduct = [WBInAppHelper isProductPaid:@"com.my.product"];
```
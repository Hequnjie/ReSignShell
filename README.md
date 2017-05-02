# ReSignShell


# iOS

iOSReSign 使用说明

iOSReSign [ipa路径] [-AppBundleIdentifier=<AppBundleIdentifier>] [-ProvisionProfilePath=<ProvisionProfilePath>] [-Certificate=<Certificate>] [-Out=<Out>] [-ResourceRules=<ResourceRules>]


-AppBundleIdentifier:   需要修改的app Bundle Identifier （可不传）
-ProvisionProfilePath:  需要使用的Provision Profile绝对路径，如果使用ipa原有的Provision Profile则不需要传递该参数 （可不传）
-Certificate:           签名App使用的证书文件名称或SHA-1值 （必要参数）
-Out:                   签名后的ipa文件目录，签名后的文件为reSign.ipa （必要参数）
-ResourceRules:         签名ipa时指定不签名的资源文件 （可不传）

Example：
./iOSReSign /Users/mac/Desktop/iOSReSign/*.ipa  -AppBundleIdentifier="com.reSignShell.test" -ProvisionProfilePath="/Users/mac/Desktop/iOSReSign/*.mobileprovision" -Certificate="4566FC00FD3********9C7EB11A" -Out="/Users/mac/Desktop/iOSReSign/out" -ResourceRules="/Users/mac/Desktop/iOSReSign/ResourceRules.plist"


# macOS

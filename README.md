Alljoyn
=======

Steps to comiple Alljoyn Framework for IOS


01. Install Command Line Tools for XCode
02. Download OpenSSL from http://www.openssl.org/ or directly from www.openssl.org/source/openssl-1.0.1e.tar.gz
03. Download the Xcode project that can be used to build OpenSSL for iOS from GitHub from the following web address: https://github.com/sqlcipher/openssl-xcode/
04. Extract downloaded project from step 2
05. Copy openssl-1.0.1e.tar.gz downloaded file in step-1 to extracted folder in step-3
06. extract openssl-1.0.1e.tar.gz in folder created in step-3
07. Open openssl.xcodeproj created in step-3
08. Build crypto for all different - different available platform
09. in X-Code find libcrypto.a under Products under openssl
10. Right click to libcrypto.a Show in finder
11. Copy parent folder's parent folder of libcrypto.a so we get lib for all version (iphonesimulator, iphoneos and mac) and for both debug and release
12. Pest that folder with build name under openssl-xcode-master created in step 3
13. set environment variable from terminal by running launchctl setenv OPENSSL_ROOT <path to top level folder containing openssl>
14. Download AllJoyn sdk from https://www.alljoyn.org/docs-and-downloads/ios-and-osx
15. Extract alljoyn-3.4.0-osx_ios-sdk.zip
16. Goto Build Settings and search Other Linker Flag Set -ObjC
17. Build alljoyn-3.4.0-osx_ios-sdk -> alljoyn_objc -> AllJoynFramework_iOS -> AllJoynFramework_iOS.xcodeproj

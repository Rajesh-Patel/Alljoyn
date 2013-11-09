Alljoyn
=======

Steps to comiple Alljoyn Framework for IOS


Install Command Line Tools for XCode
Download OpenSSL from http://www.openssl.org/ or directly from www.openssl.org/source/openssl-1.0.1e.tar.gz
Download the Xcode project that can be used to build OpenSSL for iOS from GitHub from the following web address: https://github.com/sqlcipher/openssl-xcode/
Extract downloaded project from step 2
Copy openssl-1.0.1e.tar.gz downloaded file in step-1 to extracted folder in step-3
extract openssl-1.0.1e.tar.gz in folder created in step-3
Open openssl.xcodeproj created in step-3
Build crypto for all different - different available platform
in X-Code find libcrypto.a under Products under openssl
Right click to libcrypto.a Show in finder
Copy parent folder's parent folder of libcrypto.a so we get lib for all version (iphonesimulator, iphoneos and mac) and for both debug and release
Pest that folder with build name under openssl-xcode-master created in step 3
set environment variable from terminal by running launchctl setenv OPENSSL_ROOT <path to top level folder containing openssl>
Download AllJoyn sdk from https://www.alljoyn.org/docs-and-downloads/ios-and-osx
Extract alljoyn-3.4.0-osx_ios-sdk.zip
Goto Build Settings and search Other Linker Flag Set -ObjC
Build alljoyn-3.4.0-osx_ios-sdk -> alljoyn_objc -> AllJoynFramework_iOS -> AllJoynFramework_iOS.xcodeproj

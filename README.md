# PodSpecs
This is list of private PodSpecs, which lets CocoaPods find the pod when you try to install it.
Add below source in your Podfile and then add the desired pod.
```
source 'https://github.com/satyadevchauhan/PodSpecs.git'
```
```
pod 'SampleSDK'
```

## Add Specs
Enter the following in Terminal, making sure you’re still in the framework directory you are trying to add:
```
pod repo add [YourFrameworkName] [YourPrivateSpecGitRepo]
```

The push the framework for podsec.
```
pod repo push [YourFrameworkName] [YourFrameworkName].podspec
```

### Example
```
pod repo add SampleSDK https://github.com/satyadevchauhan/PodSpecs.git
pod repo push SampleSDK SampleSDK.podspec
```

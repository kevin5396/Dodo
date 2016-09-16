# Uncomment this line to define a global platform for your project
# source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '9.0'


target 'Dodo' do
  # Comment this line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Dodo
  pod 'SCLAlertView', :git => 'https://github.com/vikmeup/SCLAlertView-Swift.git', :branch => 'swift-2.3'
  pod 'Alamofire', '~> 3.5'
  pod 'ChameleonFramework/Swift'
  pod 'Eureka', :git => 'https://github.com/xmartlabs/Eureka.git', :branch => 'swift2.3'
  pod 'Cosmos', '~> 1.2'
  pod 'XLPagerTabStrip', '~> 5.0'
  pod 'RxCocoa'
  pod 'NSObject+Rx'
  pod 'Action'
  pod 'RxSwift', :git => 'https://github.com/ReactiveX/RxSwift.git', :branch => 'rxswift-2.0'
  pod 'Moya/RxSwift'
  pod 'SwiftyJSON'
  pod 'AlamofireImage', '~> 2.0'
  pod 'Reachability', :git => 'https://github.com/ashfurrow/Reachability.git', :branch => 'frameworks'

  target 'DodoTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'DodoUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '2.3'
    end
  end
end

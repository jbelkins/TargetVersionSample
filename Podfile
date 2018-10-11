platform :ios, '11.0'

target 'TargetVersionSample' do
  use_frameworks!

  pod "Braintree"
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      # Uncomment the following to force pod deployment target to 11.0
      # I don't think this should be necessary if platform is set at top
      # config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
    end
  end
end

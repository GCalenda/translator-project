use_frameworks!

platform :ios, '12.0'

project 'TranslateExample.xcodeproj'

pod 'GoogleMLKit/Translate', '4.0.0'

target 'TranslateExample' do
end

target 'TranslateExampleObjC' do
end

# Disable signing for pods
post_install do |installer|
  installer.generated_projects.each do |project|
    project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['CODE_SIGNING_ALLOWED'] = 'NO'
         end
    end
  end
end
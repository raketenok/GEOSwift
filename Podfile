platform :ios, '8.0'

use_frameworks!

target 'GEOSwift' do
  pod 'geos', :git => 'git@github.com:GEOSwift/geos.git', :commit => 'c04f72d7efd1f12d9e986bea746314d87b7787ca'
end

target 'GEOSwiftTests' do
  pod 'geos', :git => 'git@github.com:GEOSwift/geos.git', :commit => 'c04f72d7efd1f12d9e986bea746314d87b7787ca'
end

# Workaround for Cocoapods issue #7606
post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings.delete('CODE_SIGNING_ALLOWED')
    config.build_settings.delete('CODE_SIGNING_REQUIRED')
  end
end

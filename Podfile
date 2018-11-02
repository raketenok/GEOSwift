platform :ios, '8.0'

use_frameworks!

target 'GEOSwift' do
  pod 'geos', :git => 'git@github.com:GEOSwift/geos.git', :commit => 'd3465b402d3d004b7677cb6ebe286636c600c33f'
end

target 'GEOSwiftTests' do
  pod 'geos', :git => 'git@github.com:GEOSwift/geos.git', :commit => 'd3465b402d3d004b7677cb6ebe286636c600c33f'
end

# Workaround for Cocoapods issue #7606
post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings.delete('CODE_SIGNING_ALLOWED')
    config.build_settings.delete('CODE_SIGNING_REQUIRED')
  end
end

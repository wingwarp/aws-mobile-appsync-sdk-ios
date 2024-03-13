platform :ios, "9.0"

use_frameworks!
inhibit_all_warnings!

source 'https://github.com/wingwarp/SQLiteSC.swift.git'

AWS_SDK_VERSION = "2.18.0"

target "AWSAppSync" do
  pod "AWSCore", "~> #{AWS_SDK_VERSION}"
  pod 'SQLiteSC.swift', :git => 'https://github.com/wingwarp/SQLiteSC.swift.git', :tag => '3.0.3' # :branch => 'master'
  pod "ReachabilitySwift", "~> 5.0.0"
  pod "AppSyncRealTimeClient", "~> 3.1.0"
  pod "SwiftLint"
end

target "AWSAppSyncTestCommon" do
  pod "AWSS3", "~> #{AWS_SDK_VERSION}"
  pod "ReachabilitySwift", "~> 5.0.0"
  # We directly access a database connection to verify certain initialization
  # setups
  pod 'SQLiteSC.swift', :git => 'https://github.com/wingwarp/SQLiteSC.swift.git', :branch => 'master' # :tag => '3.0.3'
  pod "AppSyncRealTimeClient", "~> 3.1.0"
end

target "AWSAppSyncTestApp" do
  pod "AWSS3", "~> #{AWS_SDK_VERSION}"
  pod "AWSMobileClient", "~> #{AWS_SDK_VERSION}"
end

target "AWSAppSyncTestHostApp" do
end

target "AWSAppSyncUnitTests" do
end

target "AWSAppSyncIntegrationTests" do
end

target "ApolloTests" do
  pod "AWSCore", "~> #{AWS_SDK_VERSION}"
end

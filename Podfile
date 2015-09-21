source 'https://github.com/CocoaPods/Specs.git'

use_frameworks!

workspace 'Meteor'

xcodeproj 'Meteor'

podspec

link_with ['Meteor', 'Server Integration Tests']

target 'Unit Tests' do
  pod 'OCMock'
end

target 'Leaderboard', exclusive: true do
  platform :ios, '7.0'
  xcodeproj 'Examples/Leaderboard/Leaderboard'
  pod 'Meteor', path: '.'
end

target 'Todos', exclusive: true do
  platform :ios, '7.0'
  xcodeproj 'Examples/Todos/Todos'
  pod 'Meteor', path: '.'
end

target 'MeteorOSX', exclusive: true do
  platform :osx, '10.10'
  xcodeproj 'Examples/MeteorOSX/MeteorOSX'
  pod 'Meteor', path: '.'
end

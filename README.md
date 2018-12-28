# Flutter for Android developers

<p align="center"><img src="https://raw.githubusercontent.com/m3sv/Flutter-introduction-for-Android-developers/master/android_flutter.png" width="480"></p> 

The tutorial assumes that you are at least familiar with Android development and know what scary words like [View](https://developer.android.com/reference/android/view/View), [ViewGroup](https://developer.android.com/reference/android/view/ViewGroup), [Java](https://www.oracle.com/technetwork/java/javase/overview/index.html), [Kotlin](https://kotlinlang.org/) mean.

# Table of contents
* [Overview of Flutter](https://github.com/m3sv/Flutter-introduction-for-Android-developers#overview-of-flutter)
* [Installing Flutter](https://github.com/m3sv/Flutter-introduction-for-Android-developers#installing-flutter)
* [Working with an editor](https://github.com/m3sv/Flutter-introduction-for-Android-developers#working-with-an-editor)
* [Learning Dart](https://github.com/m3sv/Flutter-introduction-for-Android-developers#learning-dart)
* [Flutter introductory resources](https://github.com/m3sv/Flutter-introduction-for-Android-developers#flutter-introductory-resources)
* [Architecture and state management](https://github.com/m3sv/Flutter-introduction-for-Android-developers#architecture-and-state-management)
* [Navigation & routing](https://github.com/m3sv/Flutter-introduction-for-Android-developers#navigation--routing)
* [Android functionality and corresponding plugins](https://github.com/m3sv/Flutter-introduction-for-Android-developers#android-functionality-and-corresponding-plugins)
* [Network requests and Serialization](https://github.com/m3sv/Flutter-introduction-for-Android-developers#network-requests-and-serialization)
* [Reactive/Rx](https://github.com/m3sv/Flutter-introduction-for-Android-developers#reactiverx)
* [Android views and their corresponding Flutter widgets](https://github.com/m3sv/Flutter-introduction-for-Android-developers#android-views-and-their-correspoding-flutter-widgets)
* [Animation](https://github.com/m3sv/Flutter-introduction-for-Android-developers#animations)
* [Plugins/Libraries](https://github.com/m3sv/Flutter-introduction-for-Android-developers#pluginslibraries)
* [Local notifications](https://github.com/m3sv/Flutter-introduction-for-Android-developers#local-notifications)
* [Firebase](https://github.com/m3sv/Flutter-introduction-for-Android-developers#firebase)
* [Communicating with native platform](https://github.com/m3sv/Flutter-introduction-for-Android-developers#communicating-with-native-platform)
* [Background processing](https://github.com/m3sv/Flutter-introduction-for-Android-developers#background-processing)
* [Testing and profiling](https://github.com/m3sv/Flutter-introduction-for-Android-developers#testing-and-profiling)
* [Flavors and deployment](https://github.com/m3sv/Flutter-introduction-for-Android-developers#flavors-and-deployment)
* [Samples and tutorials](https://github.com/m3sv/Flutter-introduction-for-Android-developers#samples-and-tutorials)
* [Community](https://github.com/m3sv/Flutter-introduction-for-Android-developers#community)



## Overview of Flutter

* [FAQ](https://flutter.io/docs/resources/faq)

* [Technical overview](https://flutter.io/docs/resources/technical-overview)

## Installing Flutter
* [Installing Flutter SDK](https://flutter.io/docs/get-started/install)

* [Configuring Android Studio](https://flutter.io/docs/get-started/editor)

## Working with an editor
* [Android Studio/Intellij](https://flutter.io/docs/development/tools/android-studio)
* [Visual Studio Code](https://flutter.io/docs/development/tools/vs-code)

* [Layout inspector in Flutter](https://flutter.io/docs/development/tools/inspector)

## Learning Dart
* [Overview: The Dart Language](https://www.dartlang.org/guides/language)

* [Bootstrap into Dart](https://flutter.io/docs/resources/bootstrap-into-dart)

* [Dart for Java developers Codelab](https://codelabs.developers.google.com/codelabs/from-java-to-dart/#0)

* [Dart Codelabs](https://www.dartlang.org/codelabs)

## Flutter introductory resources
* [Official Flutter docs](https://flutter.io/docs)
* [Flutter for Android developers introductory](https://flutter.io/docs/get-started/flutter-for/android-devs)

* [Google Codelab](https://codelabs.developers.google.com/codelabs/flutter/#0)

* [Tensor Programming](https://www.youtube.com/channel/UCYqCZOwHbnPwyjawKfE21wg) excelent programming videos, regularly posts Flutter tutorials

## Architecture and state management

Basically Flutter world is split between [BLoC/Rx](https://flutter.io/docs/development/data-and-backend/state-mgmt#bloc--rx)(kind of like [MVVM](https://medium.com/upday-devs/android-architecture-patterns-part-3-model-view-viewmodel-e7eeee76b73b)) and [Redux](https://flutter.io/docs/development/data-and-backend/state-mgmt#redux).
[Official documentation about state management.](https://flutter.io/docs/development/data-and-backend/state-mgmt) 

## Navigation & routing
Flutter uses [Navigator](https://docs.flutter.io/flutter/widgets/Navigator-class.html) for navigation.

[Official documentation on navigation](https://flutter.io/docs/development/ui/navigation)

## Android functionality and corresponding plugins

| Android  | Flutter  | 
|:--------:|:--------:|
[AlarmManager](https://developer.android.com/reference/android/app/AlarmManager) | [android_alarm_manager](https://github.com/flutter/plugins/tree/master/packages/android_alarm_manager)
[Intent](https://developer.android.com/guide/components/intents-filters) | [android_intent](https://developer.android.com/guide/components/intents-filters)
[Battery](https://developer.android.com/training/monitoring-device-state/battery-monitoring) | [battery](https://github.com/flutter/plugins/tree/master/packages/battery)
[Camera](https://developer.android.com/guide/topics/media/camera) | [camera](https://github.com/flutter/plugins/tree/master/packages/camera)
[Network](https://developer.android.com/training/basics/network-ops/managing) | [connectivity](https://github.com/flutter/plugins/tree/master/packages/connectivity)
[Build](https://developer.android.com/reference/android/os/Build) | [device_info](https://github.com/flutter/plugins/tree/master/packages/device_info)
[Google maps](https://developers.google.com/maps/documentation/android-sdk/intro) | [google_maps_flutter](https://github.com/flutter/plugins/tree/master/packages/google_maps_flutter)
[Google Sign-in](https://developers.google.com/identity/sign-in/android/start-integrating) | [google_sign_in](https://github.com/flutter/plugins/tree/master/packages/google_sign_in)
[Image picker](https://stackoverflow.com/questions/5309190/android-pick-images-from-gallery) |[image_picker](https://github.com/flutter/plugins/tree/master/packages/image_picker)
[Local authentication](https://developer.android.com/training/id-auth/) | [local_auth](https://github.com/flutter/plugins/tree/master/packages/local_auth)
[PackageInfo](https://developer.android.com/reference/android/content/pm/PackageInfo) | [package_info](https://github.com/flutter/plugins/tree/master/packages/package_info)
[FileProvider](https://developer.android.com/reference/android/support/v4/content/FileProvider) | [path_provider](https://github.com/flutter/plugins/tree/master/packages/path_provider)
[App shortcuts](https://developer.android.com/guide/topics/ui/shortcuts/) | [quick_actions](https://github.com/flutter/plugins/tree/master/packages/quick_actions)
[Sensors](https://developer.android.com/guide/topics/sensors/sensors_overview) | [sensors](https://github.com/flutter/plugins/tree/master/packages/sensors)
[Sharing data](https://developer.android.com/training/sharing/) | [share](https://github.com/flutter/plugins/tree/master/packages/share)
[SharedPreferences](https://developer.android.com/training/data-storage/shared-preferences) | [shared_preferences](https://github.com/flutter/plugins/tree/master/packages/shared_preferences)
[Launch URL](https://developer.android.com/guide/components/intents-common) | [url_launcher](https://github.com/flutter/plugins/tree/master/packages/url_launcher)
[ExoPlayer/MediaPlayer](https://github.com/google/ExoPlayer) |  [video_player](https://github.com/flutter/plugins/tree/master/packages/video_player)
[WebView](https://developer.android.com/reference/android/webkit/WebView) | [webview_flutter](https://github.com/flutter/plugins/tree/master/packages/webview_flutter)


## Network requests and Serialization

No, there's no Retrofit or Gson/Moshi in Flutter.

* [Fetch data from Internet](https://flutter.io/docs/cookbook/networking/fetch-data)

* [JSON serialization](https://flutter.io/docs/development/data-and-backend/json)

## Reactive/Rx
Dart is a reactive language out of box use either use Dart's [Streams](https://www.dartlang.org/tutorials/language/streams) or [RxDart](https://github.com/ReactiveX/rxdart) if you're familiar with ReactiveX.

## Android views and their correspoding Flutter widgets

Flutter contains much more widgets than Android SDK, you can discover them [here](https://flutter.io/docs/development/ui/widgets) and in [Widget index](https://flutter.io/docs/reference/widgets).

The most common Android views and their corresponding Flutter widgets are here:


| Android  | Flutter  | 
|:--------:|:--------:|
|[TextView](https://developer.android.com/reference/android/widget/TextView)  | [Text](https://docs.flutter.io/flutter/widgets/Text-class.html)
|[EditText](https://developer.android.com/reference/android/widget/EditText) | [TextField](https://docs.flutter.io/flutter/material/TextField-class.html)
|[ExpandableListView](https://developer.android.com/reference/android/widget/ExpandableListView) |[ListView](https://docs.flutter.io/flutter/widgets/ListView-class.html) + [ExpansionTile](https://flutter.io/docs/catalog/samples/expansion-tile-sample)
|[Button](https://developer.android.com/reference/android/widget/Button.html) | [RaisedButton](https://docs.flutter.io/flutter/material/RaisedButton-class.html)
|[BorderlessButton](https://developer.android.com/guide/topics/ui/controls/button#Borderless) | [FlatButton](https://docs.flutter.io/flutter/material/FlatButton-class.html)
|[CalendarView](https://developer.android.com/reference/android/widget/CalendarView)| 
|[CheckBox](https://developer.android.com/reference/android/widget/CheckBox) | [Checkbox](https://docs.flutter.io/flutter/material/Checkbox-class.html)
|[DatePicker](https://developer.android.com/reference/android/widget/DatePicker) | [showDatePicker](https://docs.flutter.io/flutter/material/showDatePicker.html) 
|[FrameLayout](https://developer.android.com/reference/android/widget/FrameLayout) |[Stack](https://docs.flutter.io/flutter/widgets/Stack-class.html)
|[GridView](https://developer.android.com/guide/topics/ui/layout/gridview) | [GridView](https://docs.flutter.io/flutter/widgets/GridView-class.html)
|[HorizontalScrollView](https://developer.android.com/reference/android/widget/HorizontalScrollView) | [ListView](https://flutter.io/docs/cookbook/lists/horizontal-list)
|[ImageButton](https://developer.android.com/reference/android/widget/ImageButton) | [RaisedButton](https://docs.flutter.io/flutter/material/RaisedButton-class.html)/[FlatButton](https://docs.flutter.io/flutter/material/FlatButton-class.html)
|[ImageView](https://developer.android.com/reference/android/widget/ImageView) | [Image](https://docs.flutter.io/flutter/widgets/Image-class.html)
|[LinearLayout](https://developer.android.com/reference/android/widget/LinearLayout) | [Column](https://docs.flutter.io/flutter/widgets/Column-class.html)/[Row](https://docs.flutter.io/flutter/widgets/Row-class.html)
|[ListView](https://developer.android.com/reference/android/widget/ListView) | [ListView](https://docs.flutter.io/flutter/widgets/ListView-class.html)
|[NumberPicker](https://developer.android.com/reference/android/widget/NumberPicker) | [Custom Widget](https://pub.dartlang.org/packages/numberpicker)
|[PopupMenu](https://developer.android.com/reference/android/widget/PopupMenu)| [PopupMenuButton](https://docs.flutter.io/flutter/material/PopupMenuButton-class.html)
|[PopupView](https://developer.android.com/reference/android/widget/PopupWindow) | [PopupMenuButton](https://docs.flutter.io/flutter/material/PopupMenuButton-class.html)
|[ProgressBar](https://developer.android.com/reference/android/widget/ProgressBar) | [LinearProgressIndicator](https://docs.flutter.io/flutter/material/LinearProgressIndicator-class.html)
|[RadioButton](https://docs.flutter.io/flutter/material/Radio-class.html)/[RadioGroup](https://developer.android.com/reference/android/widget/RadioGroup) | [Radio](https://docs.flutter.io/flutter/material/Radio-class.html)
|[RatingBar](https://developer.android.com/reference/android/widget/RatingBar) | [How to create rating bar](https://stackoverflow.com/questions/46637566/how-to-create-rating-star-bar-properly)
|[RelativeLayout](https://developer.android.com/reference/android/widget/RelativeLayout) | 
|[ScrollView](https://developer.android.com/reference/android/widget/ScrollView) | [ListView](https://docs.flutter.io/flutter/widgets/ListView-class.html)
|[SeekBar](https://developer.android.com/reference/android/widget/SeekBar) | [Slider](https://docs.flutter.io/flutter/material/Slider-class.html)
|[Spinner](https://developer.android.com/reference/android/widget/Spinner) | [DropDownButton](https://docs.flutter.io/flutter/material/DropdownButton-class.html)
|[Switch](https://developer.android.com/reference/android/widget/Switch) | [Switch](https://docs.flutter.io/flutter/material/Switch-class.html)
|[TableLayout](https://developer.android.com/reference/android/widget/TableLayout) | [Table](https://docs.flutter.io/flutter/widgets/Table-class.html)
|[TimePicker](https://developer.android.com/reference/android/widget/TimePicker) | [showDatePicker](https://docs.flutter.io/flutter/material/showDatePicker.html)
[Toast](https://developer.android.com/reference/android/widget/Toast) | [fluttertoast](https://pub.dartlang.org/packages/fluttertoast)
[Toolbar](https://developer.android.com/reference/android/widget/Toolbar) | [AppBar](https://docs.flutter.io/flutter/material/AppBar-class.html)
[RecyclerView](https://developer.android.com/reference/android/support/v7/widget/RecyclerView.html) | [ListView with ListView.builder()](https://docs.flutter.io/flutter/widgets/ListView-class.html)
[ViewPager](https://developer.android.com/reference/android/support/v4/view/ViewPager) | [PageView](https://docs.flutter.io/flutter/widgets/PageView-class.html)([Tutorial](https://iirokrankka.com/2017/09/23/bringing-the-pagetransformer-from-android-to-flutter/))
[SwipeRefreshLayout](https://developer.android.com/reference/android/support/v4/widget/SwipeRefreshLayout) | [RefreshIndicator](https://docs.flutter.io/flutter/material/RefreshIndicator-class.html)([Tutorial](https://medium.com/flutterpub/adding-swipe-to-refresh-to-flutter-app-b234534f39a7))
[CardView](https://docs.flutter.io/flutter/material/Card-class.html) | [Card](https://docs.flutter.io/flutter/material/Card-class.html)
[ConstraintLayout](https://developer.android.com/reference/android/support/constraint/ConstraintLayout) |
[CoordinatorLayout](https://developer.android.com/reference/android/support/design/widget/CoordinatorLayout) | [Scaffold](https://docs.flutter.io/flutter/material/Scaffold-class.html)
[AppBarLayout](https://developer.android.com/reference/android/support/design/widget/AppBarLayout) | [AppBar](https://docs.flutter.io/flutter/material/Scaffold-class.html) within [Scaffold](https://docs.flutter.io/flutter/material/AppBar-class.html)
[ExpandableWidget](https://developer.android.com/reference/com/google/android/material/expandable/ExpandableWidget) | [ExpansionTile](https://flutter.io/docs/catalog/samples/expansion-tile-sample)
[FloatingActionButton](https://developer.android.com/guide/topics/ui/floating-action-button) | [FloatingActionButton](https://docs.flutter.io/flutter/material/Scaffold-class.html) within [Scaffold](https://docs.flutter.io/flutter/material/FloatingActionButton-class.html)
[DrawerLayout](https://developer.android.com/reference/android/support/v4/widget/DrawerLayout) | [Drawer](https://docs.flutter.io/flutter/material/Scaffold-class.html) within [Scaffold](https://docs.flutter.io/flutter/material/Drawer-class.html)
[TabLayout](https://developer.android.com/reference/android/support/design/widget/TabLayout.html) | [TabBar](https://docs.flutter.io/flutter/material/TabBar-class.html) in conjunction with [TabBarView](https://docs.flutter.io/flutter/material/TabBarView-class.html) 
[TextInputLayout](https://developer.android.com/reference/com/google/android/material/textfield/package-summary) | [TextFormFiled](https://docs.flutter.io/flutter/material/TextFormField-class.html)
[SnackBar](https://developer.android.com/reference/android/support/design/widget/Snackbar) | [SnackBar](https://docs.flutter.io/flutter/material/SnackBar-class.html)

## Animations

* [Introduction to animations in Flutter](https://flutter.io/docs/development/ui/animations)

* [Animations tutorial](https://flutter.io/docs/development/ui/animations/tutorial)

## Plugins/Libraries 
[Packages](https://pub.dartlang.org/flutter) allow you to use Flutter packages or access underlying platform features in a form of a library.

* [Dart pub](https://pub.dartlang.org/flutter/packages)(like [Jcenter](https://bintray.com/bintray/jcenter) in Java world)
* [Official Flutter plugins from Flutter repo](https://github.com/flutter/plugins)

## Local notifications

For local notifications you would have to rely on a 3rd party plugin.

* [flutter_local_notifications](https://github.com/MaikuB/flutter_local_notifications)

* [local_notifications](https://github.com/mitchhymel/local_notifications)

## Firebase

* [Firebase entry in Flutter docs](https://flutter.io/docs/development/data-and-backend/firebase)

* [Getting started with Firebase in Flutter app](https://firebase.google.com/docs/flutter/setup)

## Communicating with native platform

* [Writing custom platform-specific code](https://flutter.io/docs/development/platform-integration/platform-channels)
* [Add Flutter to existing application](https://github.com/flutter/flutter/wiki/Add-Flutter-to-existing-apps)


## Background processing

* [Background processes](https://flutter.io/docs/development/packages-and-plugins/background-processes)
* [Executing Dart in the Background with Flutter Plugins and Geofencing](https://medium.com/flutter-io/executing-dart-in-the-background-with-flutter-plugins-and-geofencing-2b3e40a1a124)

## Testing and profiling

* [Testing](https://flutter.io/docs/testing)
* [Profiling](https://flutter.io/docs/testing/ui-performance)

## Flavors and deployment

* [Creating flavors of a Flutter app (Flutter & Android setup)](https://cogitas.net/creating-flavors-of-a-flutter-app/)

* [Flavoring Flutter](https://medium.com/@salvatoregiordanoo/flavoring-flutter-392aaa875f36)

* [Preparing for release](https://flutter.io/docs/deployment/android)

* [Fastlane continious delivery](https://flutter.io/docs/deployment/fastlane-cd)

## Samples and tutorials 

* [Flutter samples on Github](https://github.com/flutter/samples/blob/master/INDEX.md)

* [Cookbook](https://flutter.io/docs/cookbook)

* [Codelabs](https://flutter.io/docs/codelabs)

* [Tutorials](https://flutter.io/docs/reference/tutorials)

* [Flutter on Medium](https://medium.com/flutter-io)

* [Trending on Github](https://github.com/trending/dart)


## Community 

* [Reddit](https://www.reddit.com/r/FlutterDev/)

* [Gitter chat room](https://gitter.im/flutter/flutter)

* [Mailing list](flutter-dev@googlegroups.com)




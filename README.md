
<?xml version="1.0" encoding="utf-8" ?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:compileSdkVersion="28" android:compileSdkVersionCodename="9" android:installLocation="preferExternal" android:versionCode="1800" android:versionName="2.20.0" package="th.dostavista" platformBuildVersionCode="1800" platformBuildVersionName="2.20.0">
	<uses-sdk android:minSdkVersion="15" android:targetSdkVersion="28" />
	<uses-permission android:name="android.permission.WAKE_LOCK" />
	<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
	<uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
	<uses-permission android:name="android.permission.INTERNET" />
	<uses-permission android:name="android.permission.VIBRATE" />
	<uses-permission android:name="android.permission.FOREGROUND_SERVICE" />
	<uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW" />
	<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
	<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
	<uses-permission android:name="android.permission.CALL_PHONE" />
	<uses-permission android:name="android.permission.CAMERA" />
	<uses-permission android:name="android.permission.READ_PHONE_STATE" />
	<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />	<uses-feature android:name="android.hardware.camera.flash" android:required="false" />
	<uses-feature android:name="android.hardware.telephony" android:required="false" />
	<uses-feature android:name="android.hardware.camera" android:required="false" />
	<uses-feature android:name="android.hardware.camera.autofocus" android:required="false" />
	<uses-feature android:name="android.hardware.location" android:required="false" />
	<uses-feature android:name="android.hardware.location.gps" android:required="false" />
	<uses-feature android:name="android.hardware.location.network" android:required="false" />
	<uses-feature android:name="android.hardware.microphone" android:required="false" />
	<uses-feature android:glEsVersion="0x20000" android:required="true" />
	<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
	<uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" />
	<uses-permission android:name="com.google.android.c2dm.permission.RECEIVE" />
	<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE" />
	<application android:appComponentFactory="android.support.v4.app.CoreComponentFactory" android:hardwareAccelerated="true" android:icon="@drawable/ic_launcher" android:label="มิส" android:largeHeap="true" android:name="com.sebbia.delivery.DApplication" android:theme="@style/ApplicationTheme">
		<meta-data android:name="com.facebook.sdk.ApplicationId" android:value="@string/facebook_app_id" />
		<meta-data android:name="com.facebook.sdk.CodelessDebugLogEnabled" android:value="true" />
		<activity android:launchMode="singleTop" android:name="com.sebbia.debug.AppConfigDebugActivity" />
		<activity android:launchMode="singleTop" android:name="com.sebbia.debug.RouteDebugActivity" />
		<activity android:launchMode="singleTop" android:name="com.sebbia.delivery.ui.orders.OrdersActivity">
			<intent-filter>
				<action android:name="android.intent.action.MAIN" />
				<category android:name="android.intent.category.LAUNCHER" />
			</intent-filter>
			<intent-filter>
				<action android:name="delivery.ACTIVE_ORDERS" />
				<category android:name="android.intent.category.DEFAULT" />
			</intent-filter>
		</activity>
		<activity android:name="com.sebbia.delivery.ui.tests.QuizActivity" />
		<activity android:name="com.sebbia.debug.DebugActivity" />
		<activity android:name="com.sebbia.debug.ContractVisibilityActivity" />
		<activity android:name="com.sebbia.debug.OnBoardingDebugActivity" />
		<activity android:label="@string/authorization" android:name="com.sebbia.delivery.ui.authorization.NotAuthorizedActivity" />
		<activity android:label="@string/sign_up" android:name="com.sebbia.delivery.ui.authorization.RegistrationActivity" />
		<activity android:name="com.sebbia.delivery.ui.help.HelpActivity" />
		<activity android:label="@string/topics" android:name="com.sebbia.help.presentation.HelpActivity" />
		<activity android:label="@string/theme_select" android:name="com.sebbia.delivery.ui.messages.MessageTopicsActivity" />
		<activity android:label="@string/theme_select" android:name="com.sebbia.delivery.ui.messages.ReportTopicsActivity" />
                <activity android:label="@string/about_title" android:name="com.sebbia.delivery.ui.help.AboutActivity" />
		<activity android:name="com.sebbia.delivery.ui.orders.OrderDetailsActivity" android:windowSoftInputMode="stateHidden" />
		<activity android:name="com.sebbia.delivery.ui.orders.HandSignatureActivity" android:screenOrientation="landscape" />
		<activity android:label="@string/activity_title_messages" android:name="com.sebbia.delivery.ui.messages.MessagesActivity" />
		<activity android:label="@string/activity_title_new_message" android:name="com.sebbia.delivery.ui.messages.NewMessageActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/activity_title_authorization" android:name="com.sebbia.delivery.ui.authorization.AuthorizationActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/activity_title_eula" android:name="com.sebbia.delivery.ui.authorization.WebViewActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/activity_title_eula" android:name="com.sebbia.delivery.ui.authorization.AnnouncementActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/activity_title_profile" android:name="com.sebbia.delivery.ui.profile.ProfileActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/activity_title_map" android:name="com.sebbia.delivery.ui.map.MapActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/balance_activity_title" android:name="com.sebbia.delivery.ui.profile.BalanceActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:name="com.sebbia.qr_reader.QRActivity" android:noHistory="true" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/financial_delivery_activity_title" android:name="com.sebbia.delivery.ui.orders.financial.FinancialDeliveryActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:label="@string/financial_delivery_issue_select_activity_title" android:name="com.sebbia.delivery.ui.orders.financial.IssueSelectActivity" android:windowSoftInputMode="adjustResize|stateHidden" />
		<activity android:name="com.sebbia.delivery.ui.FullscreenImageActivity" />
		<activity android:name="com.sebbia.delivery.ui.profile.AddBankCardActivity" />
		<activity android:name="com.sebbia.delivery.ui.orders.TimePromiseActivity" />
		<activity android:name="com.sebbia.delivery.ui.util.SelectCustomRegionActivity" />
		<activity android:name="com.sebbia.delivery.balance.ChargeBalanceActivity" />
		<activity android:excludeFromRecents="true" android:name="com.sebbia.utils.KillingActivity" android:noHistory="true" />
		<activity android:name="com.sebbia.delivery.ui.camera.CameraActivity" />
		<service android:name="com.sebbia.delivery.location.LocationTrackingService" android:stopWithTask="false" />
		<activity android:label="@string/activity_title_select_transport" android:name="com.sebbia.delivery.ui.profile.transport.SelectTransportActivity" />
		<activity android:label="@string/recieve_confirmation" android:name="com.sebbia.delivery.ui.orders.financial.VerifyPacksActivity" />
		<activity android:label="@string/captcha_title" android:name="com.sebbia.delivery.ui.captcha.CaptchaActivity" />
		<activity android:label="@string/route_title" android:name="com.sebbia.delivery.ui.urgentpopup.UrgentOrderActivity" />
		<activity android:label="@string/app_name" android:name="com.sebbia.delivery.ui.messages.ImageActivity" />
		<activity android:name="com.sebbia.delivery.ui.orders.detail.QrScannerActivity" />
		<activity android:name="com.sebbia.delivery.ui.timeslots.TimeslotsListActivity" />
		<activity android:name="com.sebbia.delivery.ui.timeslots.TimeslotsPlacesActivity" />
		<activity android:clearTaskOnLaunch="true" android:name="com.sebbia.contract.presentation.route.RouteActivity" android:windowSoftInputMode="stateHidden" />
		<activity android:name="com.sebbia.qr_reader.barcode.BarcodeCaptureActivity" />
		<activity android:name="com.sebbia.debug.SetApiUrlActivity" />
		<receiver android:exported="true" android:name="com.appsflyer.MultipleInstallBroadcastReceiver">
			<intent-filter>
				<action android:name="com.android.vending.INSTALL_REFERRER" />
			</intent-filter>
		</receiver>
		<receiver android:name="com.sebbia.utils.InternetConnection">
			<intent-filter>
				<action android:name="android.net.conn.CONNECTIVITY_CHANGE" />
			</intent-filter>
		</receiver>
		<receiver android:exported="false" android:name="com.sebbia.delivery.analytics.NotificationDismissBroadcastReceiver" />
		<receiver android:name="com.sebbia.delivery.NotificationsAlarmReciever" />
		<service android:name="com.sebbia.delivery.notifications.FirebaseNotificationService">
			<intent-filter>
				<action android:name="com.google.firebase.MESSAGING_EVENT" />
			</intent-filter>
		</service>
		<meta-data android:name="com.google.firebase.messaging.default_notification_icon" android:resource="@drawable/icon_notification" />
		<meta-data android:name="com.google.firebase.messaging.default_notification_color" android:resource="@color/primary_dark_shadow" />
		<meta-data android:name="com.google.firebase.messaging.default_notification_channel_id" android:value="@string/app_name" />
		<meta-data android:name="com.google.android.geo.API_KEY" android:value="@string/GOOGLE_MAPS_API_KEY" />
		<meta-data android:name="io.fabric.ApiKey" android:value="4191f8afad781315a16eed682785e9b812832b96" />
		<uses-library android:name="com.google.android.maps" android:required="false" />
		<uses-library android:name="org.apache.http.legacy" android:required="false" />
		<activity android:name="com.karumi.dexter.DexterActivity" android:theme="@style/Dexter.Internal.Theme.Transparent" />
		<service android:exported="false" android:name="com.evernote.android.job.v21.PlatformJobService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<service android:exported="false" android:name="com.evernote.android.job.v14.PlatformAlarmService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<service android:exported="false" android:name="com.evernote.android.job.v14.PlatformAlarmServiceExact" />
		<receiver android:exported="false" android:name="com.evernote.android.job.v14.PlatformAlarmReceiver">
			<intent-filter>
				<action android:name="com.evernote.android.job.v14.RUN_JOB" />
				<action android:name="net.vrallev.android.job.v14.RUN_JOB" />
			</intent-filter>
		</receiver>
		<receiver android:exported="false" android:name="com.evernote.android.job.JobBootReceiver">
			<intent-filter>
				<action android:name="android.intent.action.BOOT_COMPLETED" />
				<action android:name="android.intent.action.QUICKBOOT_POWERON" />
				<action android:name="com.htc.intent.action.QUICKBOOT_POWERON" />
				<action android:name="android.intent.action.MY_PACKAGE_REPLACED" />
			</intent-filter>
		</receiver>
		<service android:exported="false" android:name="com.evernote.android.job.JobRescheduleService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<service android:exported="true" android:name="com.google.firebase.messaging.FirebaseMessagingService">
			<intent-filter android:priority="-500">
				<action android:name="com.google.firebase.MESSAGING_EVENT" />
			</intent-filter>
		</service>
		<service android:exported="false" android:name="com.google.firebase.components.ComponentDiscoveryService">
			<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.iid.Registrar" android:value="com.google.firebase.components.ComponentRegistrar" />
		</service>
		<receiver android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementReceiver" />
		<receiver android:enabled="true" android:exported="true" android:name="com.google.android.gms.measurement.AppMeasurementInstallReferrerReceiver" android:permission="android.permission.INSTALL_PACKAGES">
			<intent-filter>
				<action android:name="com.android.vending.INSTALL_REFERRER" />
			</intent-filter>
		</receiver>
		<service android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementService" />
		<service android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<receiver android:exported="true" android:name="com.google.firebase.iid.FirebaseInstanceIdReceiver" android:permission="com.google.android.c2dm.permission.SEND">
			<intent-filter>
				<action android:name="com.google.android.c2dm.intent.RECEIVE" />
			</intent-filter>
		</receiver>
		<service android:exported="true" android:name="com.google.firebase.iid.FirebaseInstanceIdService">
			<intent-filter android:priority="-500">
				<action android:name="com.google.firebase.INSTANCE_ID_EVENT" />
			</intent-filter>
		</service>
		<provider android:authorities="th.dostavista.firebaseinitprovider" android:exported="false" android:initOrder="100" android:name="com.google.firebase.provider.FirebaseInitProvider" />
		<activity android:exported="false" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:theme="@android:style/Theme.Translucent.NoTitleBar" />
		<meta-data android:name="com.google.android.gms.version" android:value="@integer/google_play_services_version" />
	</application>
</manifest>

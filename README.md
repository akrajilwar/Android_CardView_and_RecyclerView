# Android CardView and RecyclerView

CardView is another major element introduced in Material Design. Using CardView you can represent the information in a card manner with a drop shadow (elevation) and corner radius which looks consistent across the platform. CardView extends the FrameLayout and it is supported way back to Android 2.x.

![CardView - 1](https://github.com/akrajilwar/Android_CardView_and_RecyclerView/blob/master/IMG-20160810-WA001.jpg)

##How to Add CardView?

To use the CardView in your app, add the CardView dependency in build.gradle and Sync the project.

    dependencies {
      compile fileTree(dir: 'libs', include: ['*.jar'])
      compile 'com.android.support:appcompat-v7:24.1.1'
      compile 'com.android.support:cardview-v7:24.1.1'
    }
Add the <android.support.v7.widget.CardView> widget to your layout and place other UI widgets like TextViews, ImageViews inside it. You can notice that the below CardView widget contains a single TextView.

    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        xmlns:card_view="http://schemas.android.com/apk/res-auto"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:padding="16dp">

        <android.support.v7.widget.CardView
            xmlns:card_view="http://schemas.android.com/apk/res-auto"
            android:id="@+id/card_view"
            android:layout_gravity="center"
            android:layout_width="250dp"
            android:layout_height="250dp"
            card_view:cardCornerRadius="4dp">

            <TextView
                android:text="Hello Card"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:padding="10dp"/>

        </android.support.v7.widget.CardView>

    </LinearLayout>
    
    [Read full tutorial at Android Learning website](http://www.androidlearning.in/android-working-card-view-recycler-view/)

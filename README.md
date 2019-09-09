# hello-word
just another repository
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:hedgehog="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:descendantFocusability="blocksDescendants"
    android:background="#f5f5f5">

    <LinearLayout
        android:id="@+id/titleLayout"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical">

        <View
            android:id="@+id/top_view"
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:background="@color/white" />

        <RelativeLayout
            android:id="@+id/titleBar"
            android:layout_width="match_parent"
            android:layout_height="56dp"
            android:background="@color/white">

            <ImageView
                android:id="@+id/iv_back"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_centerVertical="true"
                android:layout_marginLeft="15dp"
                android:padding="8dp"
                android:src="@drawable/ic_arrow_return" />

            <TextView
                android:id="@+id/title"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_centerInParent="true"
                android:layout_gravity="center"
                android:text="预约详情"
                android:textColor="#333333"
                android:textSize="16sp" />
        </RelativeLayout>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0.5dp"
            android:layout_alignParentTop="true"
            android:background="#eeeeee" />

        <com.cmos.agentlibrary.widget.TopDialTipsView
            android:id="@+id/topDialTipsView"
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:visibility="gone" />
    </LinearLayout>

    <ScrollView
        android:id="@+id/srcoll"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/titleLayout"
        android:background="@color/color_ef4a29"
        android:layout_marginBottom="20dp">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="vertical">


            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:background="@color/white">

                <TextView
                    android:id="@+id/tvPreState"
                    android:layout_width="70dp"
                    android:layout_height="30dp"
                    android:layout_alignParentRight="true"
                    android:layout_marginRight="15dp"
                    android:layout_marginTop="15dp"
                    android:background="@drawable/textview_red_all_shape_normal"
                    android:gravity="center"
                    android:text="待执行"
                    android:textColor="#ef4a29"
                    android:textSize="14sp"
                    android:visibility="gone"/>

                <TextView
                    android:id="@+id/tvFinishState"
                    android:layout_width="70dp"
                    android:layout_height="30dp"
                    android:layout_alignParentRight="true"
                    android:layout_marginRight="15dp"
                    android:layout_marginTop="15dp"
                    android:background="@drawable/textview_green_all_shape_normal"
                    android:gravity="center"
                    android:text="已执行"
                    android:textColor="#01be72"
                    android:textSize="14sp"
                    android:visibility="gone" />

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="3dp"
                            android:layout_height="14dp"
                            android:background="#2fb5fe" />

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="客户:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvUserName"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />

                        <com.cmos.agentlibrary.widget.RatingBar
                            android:id="@+id/ratingBar"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_gravity="center_vertical"
                            android:layout_marginLeft="25dp"
                            hedgehog:clickable="false"
                            hedgehog:starCount="5"
                            hedgehog:starEmpty="@drawable/icon_ratingbar_uncheck"
                            hedgehog:starFill="@drawable/icon_ratingbar_check"
                            hedgehog:starImageSize="15dp" />
                    </LinearLayout>


                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">


                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="手机号码"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvPhoneNum"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="套餐类型:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvPackageName"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="全球通级别:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvLevel"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="呼叫时间:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvCallTime"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="主叫号码:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvForwardNo"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="被叫号码:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvPassiveNo"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <RelativeLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp">

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_centerVertical="true"

                            android:orientation="horizontal">

                            <TextView
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:text="受理号码:"
                                android:textColor="#717171"
                                android:textSize="14sp" />

                            <TextView
                                android:id="@+id/tvAcceptanceNo"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:textColor="#333333"
                                android:textSize="14sp" />

                        </LinearLayout>

                        <ImageView
                            android:id="@+id/btnModify"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_alignParentRight="true"
                            android:layout_centerVertical="true"
                            android:layout_marginRight="50dp"
                            android:background="@drawable/icon_xg"
                            android:visibility="gone" />
                    </RelativeLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="15dp"

                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="归属地:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvProvince"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginBottom="15dp"
                        android:layout_marginTop="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="状态:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvState"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:id="@+id/layoutMessage"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_alignParentRight="true"
                        android:layout_centerVertical="true"
                        android:layout_marginBottom="15dp"
                        android:orientation="horizontal">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:text="客户留言:"
                            android:textColor="#717171"
                            android:textSize="14sp" />

                        <TextView
                            android:id="@+id/tvMsg"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:textColor="#333333"
                            android:textSize="14sp" />

                        <ImageView
                            android:id="@+id/imgPlay"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginLeft="15dp"
                            android:visibility="gone" />
                    </LinearLayout>

                    <LinearLayout
                        android:id="@+id/layoutResult"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginBottom="15dp"
                        android:orientation="vertical"
                        android:visibility="gone">

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:orientation="horizontal">

                            <TextView
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:text="执行结果:"
                                android:textColor="#717171"
                                android:textSize="14sp" />

                            <TextView
                                android:id="@+id/tvResult"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:textColor="#333333"
                                android:textSize="14sp" />
                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="15dp"
                            android:orientation="horizontal">

                            <TextView
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:text="沟通结果:"
                                android:textColor="#717171"
                                android:textSize="14sp" />

                            <TextView
                                android:id="@+id/tvCommunicateResult"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="15dp"
                                android:textColor="#333333"
                                android:textSize="14sp" />
                        </LinearLayout>
                    </LinearLayout>
                </LinearLayout>
            </RelativeLayout>
        </LinearLayout>
    </ScrollView>

    <RelativeLayout
        android:id="@+id/newTaskBtn"
        android:visibility="gone"
        android:layout_width="wrap_content"
        android:layout_height="60dp"
        android:layout_below="@+id/srcoll"
        android:background="@color/white"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignParentLeft="true"
            android:layout_marginLeft="15dp"
            android:text="我的自建任务"
            android:textColor="#717171"
            android:textSize="14sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_marginRight="15dp"
            android:layout_alignParentRight="true"
            android:drawableRight="@drawable/ic_arrow_right" />
    </RelativeLayout>


    <Button
        android:id="@+id/btnCall"
        style="?android:attr/borderlessButtonStyle"
        android:visibility="gone"
        android:layout_width="match_parent"
        android:layout_height="44dp"
        android:layout_alignParentBottom="true"
        android:layout_gravity="center"
        android:layout_marginBottom="30dp"
        android:layout_marginLeft="20dp"
        android:layout_marginRight="20dp"
        android:background="@drawable/btn_checkin_all_shape_selected"
        android:text="外呼"
        android:textColor="@color/white"
        android:textSize="16sp" />


</RelativeLayout>

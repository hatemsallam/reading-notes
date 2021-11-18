# Intent Filters

* In order to properly define which intents your activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.
* The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:
  * Action : A string naming the action to perform.
  * Data : A description of the data associated with the intent.
  * Category : Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it's started.

* Each incoming intent specifies only one action and one data type, but it's OK to declare multiple instances of the `<action>`, `<category>`, and `<data>` elements in each `<intent-filter>`.

## Handle the Intent in Your Activity

* As your activity starts, call getIntent() to retrieve the Intent that started the activity.
* You can do so at any time during the lifecycle of the activity, but you should generally do so during early callbacks such as onCreate() or onStart().

## Return a Result

* simply call setResult() to specify the result code and result Intent. 
* When your operation is done and the user should return to the original activity, call finish() to close (and destroy) your activity.
* You must always specify a result code with the result.
* If you simply need to return an integer that indicates one of several result options, you can set the result code to any value higher than 0.
* If you use the result code to deliver an integer and you have no need to include the Intent
* you can call setResult() and pass only a result code. 

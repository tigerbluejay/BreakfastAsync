# BreakfastAsync
This solution contains two projects. The first “Breakfast” is a regular synchronous program that prepares breakfast, the second “BreakfastAsync” demonstrates the use of keywords async await and task, in creating an asynchronous breakfast preparation program.

The latter prepares a coffe cup and then starts fryEggsAsync() which starts off the process inside that method. When we reach the await Task.Delay(3000) command, because FryEggsAsnyc() is marked with the async keyword and is a Task that returns an egg object, execution reverts to the caller (in this case main) and FryBaconAsync() is called while we are delaying, when the await Task.Delay(3000) is done action returns to FryEggsAsync() to resume action in that method.

In this fashion, methods are called and executed asynchronously.

The Task finishedTask awaits that Tasks.WhenAny are finished (from those defined on the list) a message indicating completion should be printed.

Task is a construct to indicate work is being done on the background.

The async keyword allows for await to be used in the body of the async method.

When the await keyword is applied it suspends the calling method and yields control back to the caller.

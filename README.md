# ThreadPool
A ThreadPool library for c++



#ThreadPool examples

```c++
//a very simple task

ThreadPool th;
th.enqueue([&](){
  //do domething
});
```


```c++
//Waiting for a task and get its result

ThreadPool th;
auto taskFuture = th.enqueue([&](){
  //do domething
  //return something
});

auto ret = taskFuture.get();
```


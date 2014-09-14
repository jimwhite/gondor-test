Gondor-Base
==========

Easy way to start a Gondor-based project is to fork or clone this empty one.  See for example Gondor-Test.

The steps to initialize a working directory with this project:

```
git clone git@github.com:jimwhite/gondor-base.git
git submodule init
git submodule update
```

Where the repo url has been forked & renamed appropriately, although you can do that afterwards too of course.

Since a Gondor-based project is expected to retain the execution memos for some application, I expect you'll add one or more submodules for your application code and data.

An alternative workflow is to create a new GitHub repo (named `my-gondor-project` in this example) then:

```
git clone git@github.com:jimwhite/gondor-base.git my-gondor-project
cd my-gondor-project
git remote remove origin
git remote add origin git@github.com:yourid/my-gondor-project.git
git push -u origin master
git submodule init
git submodule update
```

Notice that the right add origin URL command will be shown on the web page for your empty GitHub project.

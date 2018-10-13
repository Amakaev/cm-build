# cm-build

Hi everyone, from thusday's merge request, a lot of changes comes to folder structure,build,serving and etc. Now Campaign Manager is hybrid Angular 6/AngularJS application, in short Angular 6 app hosts angularJS app. If u are more interested about what we are done look at this article: https://tinyurl.com/y7csrgje

present folder structure:  
./                   -> root directory of Angular cli application  
./src/ng1/fuse       -> root directory of AngularJs Fuse app  
./src/ng1/metronic   -> root directory of AngularJs Fuse app  
./src/ng1/shared     -> shared code for fuse/metronic  
./src/ng2/           -> Angular 6 app root directory  



Lets look on to serving,building proccess.
Before serving we need to install packages(for both angular's) its can be done by one command:
in root directory run following command:

`npm run install-all <fuse/metronic>`

> 'install-all' its short way to do:  
> `npm install` in root dir (for angular 6 app)  
> `npm install` in ./src/ng1/<fuse/metronic>  
> `bower install` in ./src/ng1/<fuse/metronic>  
> `bower install` in ./src/ng1/<fuse/metronic>/bower_occasional  


Serving proccess:
in root directory run following command:

`npm run start <fuse/metronic>`
will up devserver on http://localhost:4200

Building proccess:
in root directory run following command:

`npm run build <fuse/metronic> <gulp-confing-file-name>`



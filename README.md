# cm-build

Hi everyone, from thusday's merge request, a lot of changes comes to folder structure,build,serving and etc. Now Campaign Manager is hybrid Angular 6/AngularJS application, in short Angular 6 app hosts angularJS app. If u are more interested about what we are done look at this article: https://tinyurl.com/y7csrgje

Lets look on to serving,building proccess.
Before serving we need to install packages(for both angular's) its can be done by one command:
in root directory run following command:

`npm run install-all <fuse/metronic>`

Serving proccess:
in root directory run following command:

`npm run start <fuse/metronic>`
will up devserve on localhost:4200


Building proccess:
in root directory run following command:

`npm run build <fuse/metronic> <gulp-confing-file-name>`

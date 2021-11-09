# reader
    1.这是一个js调整时间差的函数
    const timeZone = { 1: 'Asia/Shanghai', 2: 'Asia/Hong_Kong', 3: 'America/New_York' }[i];
    const date = new Date(d);
    console.log(date)
    const invdate = new Date(date.toLocaleString('en-US', { timeZone }));
    console.log(invdate)
    const diff = date.getTime() - invdate.getTime();
    console.log(new Date(date.getTime() - diff))
    return new Date(date.getTime() - diff);
# setting json 的配置
"eslint.autoFixOnSave": true,  //  启用保存时自动修复,默认只支持.js文件
  "eslint.validate": [

     "javascript",  //  用eslint的规则检测js文件
     "typescript",
     {
       "language": "vue",   // 检测vue文件
       "autoFix": true   //  为vue文件开启保存自动修复的功能
     },
     {
       "language": "html",
       "autoFix": true
     },
  ],

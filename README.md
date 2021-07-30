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

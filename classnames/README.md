1. 遍历arguments然后取每一个参数
2. 如果是number或者string直接存
3. 如果是array，则递归调用，注意这里是apply
4. 如果是object，且其自身有toString的话classes.push(target.toString())
5. 否则判断是自身的属性，hasOwnProperty&&target[key],则push
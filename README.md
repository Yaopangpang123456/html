<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
        <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
        <link rel="stylesheet" href="css/liuyanban.css">
</head>
<body>
<div id="app">
        <div class="form-group">
            <textarea v-model="cont" placeholder="请输入内容"></textarea>
        </div>
        <div class="form-group" >
            <input type="button" value="添加" @click="add">
            <input type="reset" value="删除" @click="remove()">
        </div>
    <div class="content" v-for="item in arr">
        <li class="p_cont">
            <span>{{item.cont}}</span>
        </li>
    </div>

</div>
</body>
<script src="js/liuyanban.js"></script>
</html>

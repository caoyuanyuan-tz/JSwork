<template>
    <div>
        <form>
    		名字<input type="text" name="name" v-model = "name"/>
    		<br>
    		邮箱<input type="text" name="email" v-model = "email"/>
    		<br>
    		密码<input type="password" name="password" v-model = "password"/>
    		<br>
    	</form>	
    	<button id = "submit" @click="loadStudents">注册</button>
    </div>
</template>

<script>
    data():{
        return{
            name:'',
            email:'',
            password:''
        }
    },
    methods:{
        showStu(){
            console.log(this.name,this.email,this.password)
        }
    }
</script>
<template>
    <!--<div>
        <h1>Welcome to Hands on Vue.js with ASP.NET Core!</h1>
        <p>
            The time is: {{ time }}
        </p>
        <p>
            <ul>
                <li v-for="item in user" :key="item.userName">

                    UserFrom Bd {{ item.fullName }} - {{ item.userName }}

                </li>
            </ul>
        </p>
        <ProductList></ProductList>
    </div>-->
    <router-view></router-view>
</template>

<script>
    import ProductList from "./products/List.vue";
    import UserVue from "./users/User.vue";
    export default {
        name: 'app',
        components: {
            ProductList: ProductList,
            UserList: UserVue
        },
        data() {
            return {
                time: new Date().toString(),
                
            }
        },
       
}
</script>

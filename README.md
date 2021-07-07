# vue-request-axios
> This package encapsulates vue Axios request twice, including interface interception, request mode, request header, format of carrying parameters, etc., which are gathered together to simplify Axios logic code in the project and make it more concise and clear to use
# Install
> npm install vue-request-axios

# Usage
###   In the need to access the interface file to introduce:
    import vueRequestAxios from 'vue-request-axios'
### request-axios API:
    Requests can be made by passing the relevant config to vueRequestAxios.
> How to use request without parameters and request header settings
  ```
     vueRequestAxios.request({
          url:'',
          method: '',
          headers:{
          
          }
        }).then(res=>console.log(res))
  ```
  > Request to use JSON with parameters
  ```
     vueRequestAxios.request({
          url:'',
          method: '',
          params:''
        }).then(res=>console.log(res))
  ```  
  > How to use the request body with parameters
  ```
     vueRequestAxios.request({
          url:'',
          method: '',
          data:''
        }).then(res=>console.log(res))
  ```

 ### button style Constructor Options
 
 method |data|url|
 ----   |-----   | ------   | 
 get    | params | 接口地址 | 
 post   | data   | url传参  | 
 put    |                   
 delete |              
  ...   |   

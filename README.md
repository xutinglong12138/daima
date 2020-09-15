# 为什么要编写bai单元测试？
原因是单元du测试有不少的优点zhi，能够给我们的工作带来很大的帮助。
单元dao测试的优点1.帮助开发人员编写代码，提升质量、减少bug。
如果大家分析一下我们bug原因的构成，我想有会有一部分bug的原因是开发人员在编写工作代码的时候没有考虑到某些case或者边际条件。
造成这种问题的原因很多，其中很重要的一个原因是我们对工作代码所要完成的功能思考不足，而编写单元测试，特别是先写单元测试再写工作代码就可以帮助开发人员思考编写的代码到底要实现哪些功能。
例如实现一个简单的用户注册功能的业务类方法，用单元测试再写工作代码的方式来工作的话开发人员就会先考虑各种场景相关，例如正常注册、用户名重复、没有满足必要的填写内容......等
# daima
public class BubbleSortTest {

　　public static void main(String[] args) {

　　int[] arr = new int[]{-12,3,2,34,5,8,1};
　　
　　for(int i = 0;i < arr.length-1;i++){
　　　　for(int j = 0;j <arr.length-1-i;j++){
　　　　　　if(arr[j] >arr[j+1]){
　　　　　　int temp = arr[j];
　　　　　　arr[j] = arr[j+1];
　　　　　　arr[j+1] = temp;
　　　　　　}
　　　　}
　　}
  
　　for (int i = 0; i < arr.length; i++) {
　　　　System.out.println(arr[i]+"\t");
　　}

　　}
}

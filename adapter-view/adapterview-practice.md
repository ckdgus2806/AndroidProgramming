<style> 
div.polaroid {
  	width: 200px;
  	box-shadow: 0 10px 30px 0 rgba(0, 0, 0, 0.2), 0 16px 30px 0 rgba(0, 0, 0, 0.19);
  	text-align: center;
	margin-bottom: 0.5cm;
}
div.polaroid2 {
  	width: 500px;
  	box-shadow: 0 10px 30px 0 rgba(0, 0, 0, 0.2), 0 16px 30px 0 rgba(0, 0, 0, 0.19);
  	text-align: center;
	margin-bottom: 0.5cm;
}
</style>

# 어댑터 뷰  실습

- 이번 실습은 아래와 같은 커스텀 리스트 뷰를 완성하는 것임.

	<div class="polaroid">
			<img src="figure/practice-result.png" width="200"> 
	</div>
	그림1. 실습 결과 <a name="fig1"></a>
	
##1. 커스텀 리스트 뷰의 한 항목을 위한 UI 레이아웃을 구성

- 다음 그림과 같이 리스트의 한 항목을 위한 레이아웃 (**layout/item.xml**)을 정의하라.
	<div class="polaroid2">
			<img src="figure/item-layout.png"> 
	</div>

https://github.com/kwanulee/Android/blob/master/examples/CustomItemViewTest/app/src/main/res/layout/item.xml

##2. 항목의 데이터를 관리하고, 항목의 뷰를 반환하는 커스텀 어댑터 클래스 정의
https://github.com/kwanulee/Android/blob/master/examples/CustomItemViewTest/app/src/main/java/com/example/kwlee/customitemviewtest/MyItem.java

https://github.com/kwanulee/Android/blob/master/examples/CustomItemViewTest/app/src/main/java/com/example/kwlee/customitemviewtest/MyAdapter.java


https://github.com/kwanulee/Android/blob/master/examples/CustomItemViewTest/app/src/main/java/com/example/kwlee/customitemviewtest/MainActivity.java
	listView.setDivider(new ColorDrawable(Color.RED));
	listView.setDividerHeight(5);

https://github.com/kwanulee/Android/blob/master/examples/ListView/app/src/main/java/com/kwanwoo/android/listview/MainActivity.java#L30-L31
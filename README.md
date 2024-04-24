# item_modifier-set_attributes
item_modifierの1項目であるset_attributesに関するサンプルになります。

詳しくはブログ記事『[【マイクラ】set_attributesでattibute付与【item_modifier】](https://natsumake.com/item_modifier-set_attributes/)』を参考にしてください。

<h3>概要</h3>
アイテムに対してattributeを付与することが出来る、item_modifierの項目です。

<h3>使い方</h3>

データパック導入後、ワールドに入り```/reload```と入力して実行してください。

ダイヤモンドが1つ付与されるので、それを手に持った状態で以下のコマンドを実行することでattributeを付与できます。

```copy
/item modify entity @s weapon.mainhand sample:set_attribute
```

※手に持っている状態だと最大体力が20増加するようになります。<br>
そのため、サバイバルなど体力のハートが見えるゲームモードに変更して確認してください。

---

また、lootコマンドでattributesを付与されたアイテムを入手することも可能です。

```copy
/loot give @s loot sample:set_attribute
```

を実行することで、ダイヤモンドが手に入ります。

こちらは手に持っている状態である限り、防御力（防具を装備することで上がる値）が上がります。

---

そのほかのjsonファイルは、それぞれ以下の通りです。

|jsonファイル名|役割|
|--|--|
|overlap.json|複数のスロットが記載されていた場合の挙動を試せるもの|
|addition.json|operationがadditionの場合にどういう計算がなされるのかを試せるもの|
|multiply_base.json|operationがmultiply_baseの場合にどういう計算がなされるのかを試せるもの|
|multiply_total.json|operationがmultiply_totalの場合にどういう計算がなされるのかを試せるもの|

# C-
C# проверка условий
@for (int i = 0; i < Model.NewsList.Count; i=i+2)
  {
    <div class="owl-item" style="margin-left:5px">
    @Model.NewsList[i].MessageRu
    @Model.NewsList[i].Id
<hr />
    @if ((i + 1) < Model.NewsList.Count) //  если последний элемент существует
  {
    @Model.NewsList[i + 1].MessageRu
    @Model.NewsList[i + 1].Id
  }
    </div>
}

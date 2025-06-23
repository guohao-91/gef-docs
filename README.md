# gef-docs


这是一段普通的 Markdown 文本。


    这是一段普通的 Markdown 文本。
<div style="padding-left: 20px; padding-top: 30px;">
    这是一段普通的 Markdown 文本。
</div>

这是一段普通的 Markdown 文本。
<table>
  <tr>
    <td></td>
    <td>使用例</td>
    <td>変換後</td>
  </tr>
  <tr>
    <td rowspan="3">可変長引数でバインドする</td>
    <td>exp("column = ?", "15")</td>
    <td>column = '15'</td>
  </tr>
  <tr>
    <td>exp("column1 = ? AND column2 = ?", "15", "20")</td>
    <td>column1 = '15' AND column2 = '20'</td>
  </tr>
    <tr>
    <td>exp("column IN (?, ?)", "15", "20")</td>
    <td>column IN ('15', '20')</td>
  </tr>
    <tr>
    <td rowspan="2">マップでバインドする</td>
    <td>expMap("column1 = :key1 AND column2 = :key2", map)</td>
    <td>column1 = '15' AND column2 = '20'</td>
  </tr>
  <tr>
    <td>expMap("column IN (:key1, :key2)", map)</td>
    <td>column IN ('15', '20')</td>
  </tr>
</table>

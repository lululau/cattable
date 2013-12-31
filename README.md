# cattable

## 用法


`cattable -d 列分隔符 -i 表格的ID -c 列 <HTML files> `

  本工具是将指定的HTML文件中的表格按照指定的列分隔符按行列格式打印到标准输出.

  如果没有指定列分隔符，则使用`\t`; 如果没有指定输入文件，则从stdin读取输入.

  如果没有指定表格ID，则会解析并打印找到的第一个表格.

## 示例

<table id="cattable-test-table">
<thead>
<tr>
	<td>用户名</td>
	<td>Email</td>
	<td>角色</td>
	<td>锁定</td>
	<td>最后登录</td>
</tr>
</thead>
<tbody>
<tr>
	<td>Steve Jobs</td>
	<td>steve.jobs@apple.com</td>
	<td>Admin</td>
	<td>否</td>
	<td>2012-12-20 10:10</td>
</tr>
<tr>
	<td>Bill Gates</td>
	<td>bill.gates@microsoft.com</td>
	<td>Manager</td>
	<td>是</td>
	<td>2011-2-12 21:46</td>
</tr>
<tr>
	<td>Jeff Bezos</td>
	<td>jeff.bezos@amazon.com</td>
	<td>Normal</td>
	<td>否</td>
	<td>2013-5-13 08:09</td>
</tr>
</tbody>
</table>


![image](http://imglf1.ph.126.net/HbL8CkQXhm7MpCm-VEbM_A==/2259118163179861885.png)

## 安装

```
git clone https://github.com/lululau/cattable
cd cattable
sudo cp cattable /usr/local/bin/
sudo cpan HTML::TableExtract

cattable --help
```
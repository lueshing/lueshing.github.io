<html>

<head>
<meta http-equiv="Content-Type" content="text/html; charset=windows-1252">
<title>Startpage</title>
<style>
td.heading-1 { background-color:#C0C0C0; font-family: Arial; font-size: 9pt; font-weight: bold; }
td.body-1 { background-color:#F4F4F4; font-family: Arial; font-size: 7pt; vertical-align: top; }

a.href-1:active  { color:maroon; text-decoration:none;font-family:Arial;font-size:7.5pt; }
a.href-1:link    { color:maroon; text-decoration:none;font-family:Arial;font-size:7.5pt; }
a.href-1:visited { color:maroon; text-decoration:none;font-family:Arial;font-size:7.5pt; }
a.href-1:hover   { color:black; text-decoration: underline;font-family:Arial;font-size:7.5pt; }
</style>

<script language="JavaScript" src="links.js"></script>

<script language="JavaScript">
searchEngineArray = new Array();
searchEngineArray.push(new Array('http://www.google.com/search', 'q', 'Google'));
searchEngineArray.push(new Array('http://www.bing.com', 'q', 'Bing'));
searchEngineArray.push(new Array('http://search.yahoo.com/bin/search', 'p', 'Yahoo'));
searchEngineArray.push(new Array('http://www.google.com/groups', 'q', 'Google Groups'));
searchEngineArray.push(new Array('http://www.dictionary.com/search', 'q', 'dictionary.com'));

function changeEngine(num)
{	if (num == "URL") { document.forms[0].elements[0].focus(); return; }
	index = parseInt(num);
	document.forms[0].action = searchEngineArray[index][0];
	document.forms[0].elements[0].name = searchEngineArray[index][1];
	document.forms[0].elements[0].focus();
}

function redirect(blah)
{
	if (document.forms[0].blah.value != "URL") return true;

 	return false;
}

function redirectURL(blah)
{
	if (blah.indexOf("http://") == -1)
	{  window.location.href = "http://" + blah; }
  	else
  	{ window.location.href = blah; }

		return false;
}
</script>
</head>

<body topmargin="0" leftmargin="0" onLoad = "document.forms[0].elements[0].focus();">
<table border="0" cellpadding="2" style="" bordercolor="#111111" id="AutoNumber1" cellspacing="1">
  <tr>
    <td valign="top">
    <form action="http://www.google.com/search" name="searchform" style="margin-top:0px;margin-bottom:0px;" onSubmit="return redirect(document.forms[0].elements[0].value)">
    <input maxlength=256 name=q size=20 style="font-size: 7pt;">
    <select name="blah" onChange="changeEngine(value)" style="font-size: 7pt;">
<script language="JavaScript" type="text/javascript">
<!--
for(i=0; i < searchEngineArray.length; i++) {
  document.write("<option value='"+i+"'>"+searchEngineArray[i][2]+"</option>");
}
//-->
</script>

    </select>
    <input name=goog type=button value="Google" style="font-size: 7pt;" onClick="changeEngine(0);submit();">
    <input name=bing type=button value="Bing" style="font-size: 7pt;" onClick="changeEngine(1);submit();">
<!--    <input name=btnG type=submit value="Search" style="font-size: 7pt;"> -->
    </form>
    </td>
    <td valign="top">
    <form style="margin-top:0px;margin-bottom:0px;"  onSubmit="return redirectURL(theURL.value)">
    <font face="Arial" size=2><b>URL: </b></font>
    <input maxlength=256 name="theURL" size=50 style="font-size: 7pt;">
    <input name=btnG type=Submit value="Go!" style="font-size: 7pt;" onClick="redirectURL(theURL.value)">
		</form>
    </td>
  </tr>
</table>

<table border="0" cellpadding="0" style="" bordercolor="#111111" id="AutoNumber1" cellspacing="1">
  <tr>
    <td width="300" valign="top">
<script language="JavaScript">
for(i=0; i < headingArray1.length; i++)
{	document.write("<table border='0' cellspacing='1' width='100%'>");
	document.write("  <tr><td width='100%' class='heading-1'>&nbsp;" + headingArray1[i] + "</td></tr> ");
 	document.write("</table>");

    document.write("<table border='0' cellspacing='1' width='100%'><tr>");
    document.write("<td width='50%' class='body-1'>");
	for (j=0; j<subCatArray1[i].length/2; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray1[i][j][1] + "'>" + subCatArray1[i][j][0] + "</a>");
		if (j != subCatArray1[i].length/2-1)
		{	document.write("<br>");
		}
	}
    document.write("</td><td width='50%' class='body-1'>");
	for (j=Math.round(subCatArray1[i].length/2); j<subCatArray1[i].length; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray1[i][j][1] + "'>" + subCatArray1[i][j][0] + "</a>");
		if (j != subCatArray1[i].length-1)
		{	document.write("<br>");
		}
	}

    document.write("</td></tr></table>");
}
</script>
    <td valign="top">
    </td>

    <td width="300" valign="top">
<script language="JavaScript">
for(i=0; i < headingArray2.length; i++)
{	document.write("<table border='0' cellspacing='1' width='100%'>");
	document.write("  <tr><td width='100%' class='heading-1'>&nbsp;" + headingArray2[i] + "</td></tr> ");
 	document.write("</table>");

    document.write("<table border='0' cellspacing='1' width='100%'><tr>");
    document.write("<td width='50%' class='body-1'>");
	for (j=0; j<subCatArray2[i].length/2; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray2[i][j][1] + "'>" + subCatArray2[i][j][0] + "</a>");
		if (j != subCatArray2[i].length/2-1)
		{	document.write("<br>");
		}
	}
    document.write("</td><td width='50%' class='body-1'>");
	for (j=Math.round(subCatArray2[i].length/2); j<subCatArray2[i].length; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray2[i][j][1] + "'>" + subCatArray2[i][j][0] + "</a>");
		if (j != subCatArray2[i].length-1)
		{	document.write("<br>");
		}
	}

    document.write("</td></tr></table>");
}
</script>
    <td valign="top">
    </td>

    <td width="300" valign="top">
<script language="JavaScript">
for(i=0; i < headingArray3.length; i++)
{	document.write("<table border='0' cellspacing='1' width='100%'>");
	document.write("  <tr><td width='100%' class='heading-1'>&nbsp;" + headingArray3[i] + "</td></tr> ");
 	document.write("</table>");

    document.write("<table border='0' cellspacing='1' width='100%'><tr>");
    document.write("<td width='50%' class='body-1'>");
	for (j=0; j<subCatArray3[i].length/2; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray3[i][j][1] + "'>" + subCatArray3[i][j][0] + "</a>");
		if (j != subCatArray3[i].length/2-1)
		{	document.write("<br>");
		}
	}
    document.write("</td><td width='50%' class='body-1'>");
	for (j=Math.round(subCatArray3[i].length/2); j<subCatArray3[i].length; j++)
	{
		document.write("<a class='href-1' href='" + subCatArray3[i][j][1] + "'>" + subCatArray3[i][j][0] + "</a>");
		if (j != subCatArray3[i].length-1)
		{	document.write("<br>");
		}
	}

    document.write("</td></tr></table>");
}
</script>
    <td valign="top">
    </td>


  </tr>
</table>



</body>

</html>

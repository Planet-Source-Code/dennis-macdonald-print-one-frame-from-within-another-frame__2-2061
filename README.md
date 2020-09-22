<div align="center">

## Print one frame from within another frame


</div>

### Description

This JavaScript code fragment allows you to print print one frame from a button ect within another frame on the same page.
 
### More Info
 
None known.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Dennis Macdonald](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dennis-macdonald.md)
**Level**          |Intermediate
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |
**Category**       |[Browser/ System Services](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/browser-system-services__2-69.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dennis-macdonald-print-one-frame-from-within-another-frame__2-2061/archive/master.zip)





### Source Code

```
In your frame page, make FrameA and FrameB the frame names. HTML for framer page below:
<frameset rows="20%,*">
<frame SRC="framea.htm" name="FrameA" noresize>
<frame SRC="frameb.htm" name="FrameB" noresize>
<noframes>
<body>
</body>
</noframes>
</frameset>
</html>
HTML for FrameA.htm page below:
<html>
<head>
<script>
function PrintOtherFrame(){
 parent.FrameB.focus();
 window.print();
}
</script>
</head>
<body>
<form name="formA"><input type="button" value="Print the other frame" onclick="PrintOtherFrame()">
</body>
</html>
HTML for FrameB.htm page below:
<html>
<head>
</head>
<body>
....
.... whatever you like
....
</body>
</html>
```


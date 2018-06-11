@{
    ViewBag.Title = "About";
}
<h2>@ViewBag.Title.</h2>
<h3>@ViewBag.Message</h3>

<p>Use this area to provide additional information.</p>
 
<input type="text" id="pasteIt" /> 
<script src="~/Scripts/jquery-1.10.2.min.js"></script>
 
<script>
  
    $(document).on('paste', '#pasteIt', function (e) {        
        e.preventDefault();
        // prevent copying action
        alert(e.originalEvent.clipboardData.getData('Text'));
        var withoutSpaces = e.originalEvent.clipboardData.getData('Text');
        withoutSpaces = withoutSpaces.replace(/\s+/g, '');
        $(this).val(withoutSpaces);
        // you need to use val() not text()
    });
    $(document).on('paste', '#pasteIt', function (e) {
        e.preventDefault();
        // prevent copying action
        alert(e.originalEvent.clipboardData.getData('Text'));
        var withoutSpaces = e.originalEvent.clipboardData.getData('Text');
        withoutSpaces = withoutSpaces.replace(/\s+/g, '');
        $(this).val(withoutSpaces);
        // you need to use val() not text()
    });
</script># Testropository
this is for test

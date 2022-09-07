 // Create an HTML Form by using native HTML API
using (var document = new Aspose.Html.HTMLDocument())
{
    var editor = Aspose.Html.Forms.FormEditor.CreateNew(document);
    var body = document.Body;

    // create form-element
    var form = (HTMLFormElement)document.CreateElement("form");
//                form.Action = "action_page.php";

    // Create FirstName label
    var label = (HTMLLabelElement)document.CreateElement("label");
    label.TextContent = "First name:";
    label.For = "fname";
    form.AppendChild(label);
    form.AppendChild(document.CreateElement("br"));

    // Create FirstName field
    var input = (HTMLInputElement)document.CreateElement("input");
    input.Type = "text";
    input.Id = "fname";
    input.Name = "fname";
    form.AppendChild(input);
    form.AppendChild(document.CreateElement("br"));
    form.AppendChild(document.CreateElement("br"));
		}

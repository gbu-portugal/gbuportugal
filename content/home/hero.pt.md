+++
# Hero widget.
widget = "hero"
active = true
date = 2017-10-15T00:00:00

title = "Temos uma nova política de privacidade"

# Order that this section will appear in.
weight = 3

# Overlay a color or image (optional).
#   Deactivate an option by commenting out the line, prefixing it with `#`.
[header]
  overlay_color = "#666"  # An HTML color value.
  overlay_img = ""  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

# Call to action button (optional).
#   Activate the button by specifying a URL and button label below.
#   Deactivate by commenting out parameters, prefixing lines with `#`.
[cta]
  url = "./page/politica-privacidade/"
  label = '<i class="fa "></i>Política de Privacidade do GBU'
+++

Conhece as alterações:

<script type="text/javascript">
  (function defer() {
    if (window.jQuery) {
      jQuery(document).ready(function(){
        GetLatestReleaseInfo();
      });
    } else {
      setTimeout(function() { defer() }, 50);
    }
  })();  
  function GetLatestReleaseInfo() {
    $.getJSON('https://api.github.com/repos/gcushen/hugo-academic/tags').done(function (json) {
      let release = json[0];
      // let downloadURL = release.zipball_url;
      $('#academic-release').text('Latest release ' + release.name);  
    });    
}  
</script>

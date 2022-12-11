---
title: ComponentGuid (Simple Type)
layout: documentation_xsd_simpletype
---
<dl>
  <dt>Description</dt>
  <dd>Values of this type will look like: `01234567-89AB-CDEF-0123-456789ABCDEF` or `{'{'}01234567-89AB-CDEF-0123-456789ABCDEF{'}'}`, but also allows "PUT-GUID-HERE" for use in examples.  It's also possible to have an empty value "".</dd>
  <dt>Pattern Type</dt>
  <dd>Must match the regular expression: '[{'{'}(]?[0-9A-Fa-f]{'{'}8{'}'}\-?[0-9A-Fa-f]{'{'}4{'}'}\-?[0-9A-Fa-f]{'{'}4{'}'}\-?[0-9A-Fa-f]{'{'}4{'}'}\-?[0-9A-Fa-f]{'{'}12{'}'}[{'}'})]?|[{'{'}(]?\?{'{'}8{'}'}\-\?{'{'}4{'}'}\-\?{'{'}4{'}'}\-\?{'{'}4{'}'}\-\?{'{'}12{'}'}[{'}'})]?|PUT\-GUID\-(\d+\-)?HERE|([!$])(\(var|\(loc|\(wix)\.[_A-Za-z][0-9A-Za-z_.]*\)|\*|^$'.</dd>
  <dt>See Also</dt>
  <dd>
    <a href="../">Gaming Schema</a>
  </dd>
</dl>
# https-only


add below code in head tag to forcefully redirect user to https only

    <script>
        var protocol = location.protocol
        if (protocol == "http:") {
            var link_without_protocol = location.hostname + location.pathname + location.hash
            var secure_link = 'https://' + link_without_protocol
            window.location = secure_link
        }
    </script>
    
    
    
    

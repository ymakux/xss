$filter = new Filter();

$allowed_protocols = array('http', 'ftp', 'mailto');
$allowed_tags = array('a', 'i', 'b', 'em', 'span', 'strong', 'ul', 'ol', 'li', 'table', 'tr', 'td', 'thead', 'th', 'tbody');

$filter->addAllowedProtocols($allowed_protocols);
$filter->addAllowedTags($allowed_tags);

$filtered_string = $filter->xss($string);
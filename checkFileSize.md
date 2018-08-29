# Get Filesize in KB,MB,GB when filesize in bytes

>
    function filesize($bytes)
    {
        if ($bytes >= 1073741824)
        {
            $bytes = number_format($bytes / 1073741824, 2) . ' GB';
        }
        elseif ($bytes >= 1048576)
        {
            $bytes = number_format($bytes / 1048576, 2) . ' MB';
        }
        elseif ($bytes >= 1024)
        {
            $bytes = number_format($bytes / 1024, 2) . ' KB';
        }
        elseif ($bytes > 1)
        {
            $bytes = $bytes . ' bytes';
        }
        elseif ($bytes == 1)
        {
            $bytes = $bytes . ' byte';
        }
        else
        {
            $bytes = '0 bytes';
        }

        return $bytes;
    }


    // @getFilesize() reqired two parameters @size and @option

	function getFilesize($size, $option)
	{
		
		// @size = file size in bytes
		// @option = KB,MB,GB
		$finalSize = 0;
		switch ($option) {
			case 'KB':
				$finalSize = number_format($size / 1024, 2);
				break;
			case 'MB':
				$finalSize = number_format($size / 1048576, 2);
				break;
			case 'GB':
				$finalSize = number_format($size / 1024, 2);
				break;
			
			default:
				break;
		}

		return $finalSize;
	}


# This is to create a certificate request for iis hosted domains

# Defining parameters for request files in/out path
param [

[Parameter(Mandatory=$True,Position=1)]
[string] $requestFilesPath,

[Parameter(Mandatory=$false,Position=2)]
[string] $requestOutFilesPath,

[Parameter(Mandatory=$false,Position=3)]
[string] $requestOutFolderName

]

# Get each name in the request files path
$requestFiles = (Get-ChildItem -Path $requestFilesPath).Name

cd $requestFilesPath
New-Item -Name $requestOutFolderName -ItemType folder

# Run a certreq for each item in the $requestFilesPath
$requestOutFiles = foreach ($item in $requestFiles) {

    $outFileName = -join($item, '.req')
    
    if($requestOutFilesPath = $true) {

        $newOutFilePath = -join($requestOutFilesPath, $outFileName)
        certreq -new $item $newOutFilePath
        $consoleCommnet = -join('new item created at: ', $newOutFilePath)
        echo $consoleCommnet
    
    }

    else {
    
        certreq -new $item $outFileName
        $outFileName = -join($requestFilesPath, '\', '$item')
        $consoleCommnet = -join('new item created at: ', $outFileName)
        echo $consoleCommnet
    
    }
}

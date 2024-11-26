# Text
# copy the text underneath
<?xml version="1.0" encoding="utf-8"?>
<unattend xmlns="urn:schemas-microsoft-com:unattend">
    <settings pass="windowsPE">
        <component name="Microsoft-Windows-Setup" processorArchitecture="x64" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="nonSxS">
            <ImageInstall>
                <OSImage>
                    <InstallFrom>
                        <MetaData wcm:action="add">
                            <Key>/image/index</Key>
                            <Value>1</Value>
                        </MetaData>
                    </InstallFrom>
                </OSImage>
            </ImageInstall>
            <UserData>
                <AcceptEula>true</AcceptEula>
                <FullName>Benutzername</FullName>
                <Organization>Organisation</Organization>
            </UserData>
        </component>
    </settings>
    <settings pass="specialize">
        <component name="Microsoft-Windows-Shell-Setup" processorArchitecture="x64" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="nonSxS">
            <ProductKey>XXXX-XXXX-XXXX-XXXX</ProductKey>
            <TimeZone>W. Europe Standard Time</TimeZone>
        </component>
    </settings>
    <settings pass="oobeSystem">
        <component name="Microsoft-Windows-Shell-Setup" processorArchitecture="x64" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="nonSxS">
            <OOBE>
                <HideEULAPage>true</HideEULAPage>
                <NetworkLocation>Work</NetworkLocation>
                <ProtectYourPC>3</ProtectYourPC>
            </OOBE>
            <UserAccounts>
                <AdministratorPassword>
                    <Value>PASSWORD</Value>
                    <PlainText>true</PlainText>
                </AdministratorPassword>
            </UserAccounts>
        </component>
    </settings>
</unattend>


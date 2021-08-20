workspace "Sample Connect" "Sample Connect solution" {

    model {

        //users

        rUser = person "rUser" ""

        oUser = person "oUser"

        //client  systems
        customerFTPServer = softwareSystem "Customer FTP Server" "FTP"
        customerSFTPServer = softwareSystem "Customer SFTP Server" "FTP"
        customerFileSystem = softwareSystem "Customer File system (local)" "Folder" "Folder"
        customerPrinter = softwareSystem "Customer Printer" "Printer" "Printer"

        enterprise "Software" {

            //infrastructure systems
            emailprovider = softwareSystem "Email System" "Email"
            SFTPServer = softwareSystem "SFTP Server" "FTP"

            //software systems

            System1 = softwareSystem "System 1" "System 1" {
                ClientContainer1 = container " Browser" "Embedded Browser" "WebBrowswer" "WebBrowser"
            }

            ConnectSystem = softwareSystem "NOVConnect" "NOVConnect" {
                ConfigToolContainer = container "Config Tool" "C#" "Windows App"
                dataSourcesContainer = container "DataSources" "C#" "Windows Process"
                databaseContainer = container "MainDatabase" "Main System Database" "SQL Server Database Schema" "Database"
                
            }

        }        
    }     
    views {

        //overall diagram
        systemLandscape "WellDataSystem" "This is the overview of WellData" {
            include *
            autoLayout
        }

     

        styles {
            element "Element" {
                color #ffffff
                background #5B9BD5
            }
            element "Software System" {
                background #801515
                shape RoundedBox
            }
            element "WellData System" {
                background #550000
                color #ffffff
            }

            element "Future State" {
                opacity 30
            }
            element "Person" {
                background #d46a6a
                shape Person
            }
            relationship "Relationship" {
                dashed false
            }
            relationship "Asynchronous" {
                dashed true
            }
            relationship "Alert" {
                color #ff0000
            }
            relationship "Future State" {
                opacity 30
            }
            element "Database" {
                shape Cylinder
                background #5B9BD5
            }

            element "Folder" {
                shape Folder
                background #5B9BD5
            }

            element "Printer" {
                shape Robot
                background #5B9BD5
            }

            element "WebBrowser" {
                shape WebBrowser
                background #5B9BD5
            }
            element "MobileDevicePortrait" {
                shape MobileDeviceLandscape
                background #5B9BD5
            }

            element "New" {
                background #d46a6a
            }

       }
    }
}   

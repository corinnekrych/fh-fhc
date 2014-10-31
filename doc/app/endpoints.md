fhc-endpoints(1)
================
## SYNOPSIS

 fhc app endpoints --app=<app> --env=<env>

## EXAMPLES

  fhc version                                                                                                
  fhc app act --app=1a2b3c --fn=<serverside Function> --data=<data to send> --env=<environment>              Performs an act request on app with id 1a2b3c
  fhc app cloud --app=1a2b3c --path=<serverside path from root> --data=<Data to send> --env=<environment>    Performs a cloud request on app with id 1a2b3c
  fhc app create --project=1a2b3c --title=My New App --type=cloud_nodejs                                     Creates a new hybrid app
  fhc app delete --project=1a --app=2b                                                                       Deletes app with id 2b under project with id 1a
  fhc app endpoints --app=1a2b --env=dev                                                                     Lists all endpoints exposed by app with guid 1a2b in the dev environment


## OPTIONS

  --data       Request body to send thru                                                                      [required]
  --fn         Cloud function name to call                                                                    [required]
  --path       Path of the cloud request                                                                      [required]
  --title, -t  A title for your app                                                                         
  --type, -y   Type of your app - e.g. client_hybrid, client_native_ios, client_native_android, cloud_nodejs  [default: "client_hybrid"]

## DESCRIPTION

Provides the endpoints for the specified app in the specified environment.

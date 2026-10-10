| legacy | 192.168.0.0/16 | 192.168.0.1 | 65534 | old network |

# Network Specification

 ## Networks
 
 | Name     | CIDR          | Gateway    | Hosts | Purpose                  |
 |----------|---------------|------------|-------|--------------------------| 
 | frontend | 172.20.0.0/24 | 172.20.0.1 | 254   | Public services (web)    | 
<<<<<<< HEAD
 | backend  | 172.22.0.0/24 | 172.21.0.1 | 254   | Internal (API, database) |
=======
 | backend  | 172.21.0.0/25 | 172.21.0.1 | 254   | Internal (API, database) |
>>>>>>> feature/backend-a
 
  ## Rules 
  
  - The frontend and backend networks must not overlap. 
  - Only services on the frontend network are exposed to users.
  - The database is connected to the backend network only.
  
  ## Change history 
  
  This file is managed with Git. Run: git log network/network.mdgitdraft: add a management network

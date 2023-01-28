# elasticsearch


Run the below command to run the Elastic Search in your kuberntes Cluster:

Make sure you are having 2GB RAM Free in your cluster node, otherwise you will get OOMKILLED Error.

          kubectl apply -f config.yaml
          
          kubectl apply -f deployment.yaml
          
          kubectl apply -f service.yaml
          
          
Validate the elastic search up and running

          use KubeForwared  and open the port 9200 with db service
          
          access the url: http://localhost:9200
          
          You should see the below screen shot
          
                  {
                    "name" : "elasticsearch-85476ccc9-nfmfx",
                    "cluster_name" : "elasticsearch",
                    "cluster_uuid" : "2pVNoa5LQseDW3G-MVZMog",
                    "version" : {
                      "number" : "8.5.2",
                      "build_flavor" : "default",
                      "build_type" : "docker",
                      "build_hash" : "a846182fa16b4ebfcc89aa3c11a11fd5adf3de04",
                      "build_date" : "2022-11-17T18:56:17.538630285Z",
                      "build_snapshot" : false,
                      "lucene_version" : "9.4.1",
                      "minimum_wire_compatibility_version" : "7.17.0",
                      "minimum_index_compatibility_version" : "7.0.0"
                  },
                  "tagline" : "You Know, for Search"
                }


Install Elastic Vue in your chrome browser and enable: 

                chrome://extensions/
                
                And configure your local cluster using http://localhost:9200/
                
                Then you will see the below response on the screen

<img width="1728" alt="image" src="https://user-images.githubusercontent.com/109475849/215254979-ffaf4d4c-ba84-4781-aa6b-d358649f26f6.png">


# Sandbox for maps 

    wget https://hiu.state.gov/data/Global_Points_2013March12_HIU_USDoS.zip
    unzip Global_Points_2013March12_HIU_USDoS.zip
    ogr2ogr -f GeoJSON Global_Points_2013March12_HIU_USDoS.geojson Global_Points_2013March12_HIU_USDoS.shp
    topojson -o Global_Points_2013March12_HIU_USDoS.json Global_Points_2013March12_HIU_USDoS.geojson
    mkdir build 
    cd build 
    curl -O https://hiu.state.gov/data/Syria_RefugeeCamps_2013May29_HIU_USDoS.zip
    unzip Syria_RefugeeCamps_2013May29_HIU_USDoS.zip
    cd ..
    ogr2ogr -f GeoJSON Syria_RefugeeCamps_2013May29_HIU_USDoS.geojson build/Syria_RefugeeCamps_2013May29_HIU_USDoS.shp
    


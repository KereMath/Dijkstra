#include "the7.h"

int Distance(int dst[], bool visited[], int n,std::vector<int>pathneed )
{
 
    int min = INT_MAX, index;
 
    for (int v = 0; v < n; v++)
        if (visited[v] == false && dst[v] <= min){
            min = dst[v], index = v;
     }
            
 
    return index;
}

void CanCatch(int n, std::vector<Road> roads, int s, int d, int x, int y, int l, int printPath) {
    // You can change these variables. These are here for demo only.
    std::vector<int> path;
    std::vector<int> path1;
    
    int prev[n];
    int prev1[n];
    int prev2[n];
    int prev3[n];
    int prev4[n];
    int prev5[n];
    int prev6[n];
    
    int G[n][n];
    for(int i=0;i<n;i++){
        for(int j=0;j<n;j++){
            G[i][j]=0;
        }
    }
    int a,b,c;
    int t=roads.size();
    for(int j=0;j<t;j++){
        c=roads[j].time;
        a=roads[j].buildings.first;
        b=roads[j].buildings.second;
        G[a][b]=c;
        G[b][a]=c;
    }
    int dist[n];
    int dist1[n];
    bool visited[n]; 
   
    for (int i = 0; i < n; i++){
        dist1[i] = INT_MAX, visited[i] = false;}
 
    dist1[s] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist1, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist1[u] != INT_MAX
                && dist1[u] + G[u][v] < dist1[v]){
                dist1[v] = dist1[u] + G[u][v];
                prev[v]=u;
                if(v!=x){
                    prev1[v]=u;
                   
                }
                if(v==x){
                    prev1[v]=u;
                  
                }
                if(v!=y){
                    prev2[v]=u;
                    
                }
                if(v==y){
                    prev2[v]=u;
                   
                }
            
                if(v==d){
                break;}
               
             

                }}
    }
    int val4=0;
    int val5=0;
 
    int val3=dist1[d];
    int val1=dist1[x];
    int val2=dist1[y];
    int val6=dist1[x];
    int val7=dist1[y];
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[x] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                if(v!=y){prev3[v]=u;}
            
                    if(v==y){prev3[v]=u;
                break;}
                    
                }}
    }
    val1+=dist[y];
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[y] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                if(v!=d){prev4[v]=u;}
                    if(v==d){   prev4[v]=u;
                break;}
                    
                }}
    }
    val1+=dist[d];
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[y] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                if(v!=x){
                prev5[v]=u;}
                    if(v==x){ prev5[v]=u;
                break;}
                    
                }}
    }
    val2+=dist[x];
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[x] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                if(v!=d){prev6[v]=u;}
                    if(v==d){   prev6[v]=u;
                break;}
                   
                }}
    }
    val2+=dist[d];
    
    
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[x] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                prev1[v]=u;
                    if(v==d){ 
                break;}
                }}
    }
    val4=val6+dist[d];
    for (int i = 0; i < n; i++){
        dist[i] = INT_MAX, visited[i] = false;}
 
    dist[y] = 0;

    for (int count = 0; count < n - 1; count++) {
  
        int u = Distance(dist, visited, n, path);
 
        visited[u] = true;

        for (int v = 0; v < n; v++){
            if (!visited[v] && G[u][v]
                && dist[u] != INT_MAX
                && dist[u] + G[u][v] < dist[v]){
                dist[v] = dist[u] + G[u][v];
                prev2[v]=u;
                    if(v==d){  
                break;}
                }}
    }
    val5=dist[d]+val7;
    if(val3>l){
        std::cout<<"IMPOSSIBLE"<<std::endl;
    }
    
    
    
    
    
    
    else if(val1<=l && val1<=val2){
        std::cout<<"YES BOTH "<< val1 <<"MINUTES"<<std::endl;
        int i=d;
        path1.push_back(d);
        while(i!=y){
            path1.push_back(prev4[i]);
            i=prev4[i];
        }
        int j=y;
        
        while(j!=x){
            path1.push_back(prev3[j]);
            j=prev3[j];
        }
        int u=x;
        while(u!=s){
            path1.push_back(prev[u]);
            u=prev[u];
        }
       
         for(int m=1;m<=path1.size();m++){
            path.push_back(path1[path1.size()-m]);
        }
   
        
        
        
        if(printPath){
    PrintRange(path.begin(), path.end());
    }}
    
    
    
    
    
    else if(val2<=l && val2<=val1){
        std::cout<<"YES BOTH "<< val2 <<"MINUTES"<<std::endl;
        
        int i=d;
        path1.push_back(d);
        while(i!=x){
            path1.push_back(prev6[i]);
            i=prev6[i];
        }
        int j=x;
        
        while(j!=y){
            path1.push_back(prev5[j]);
            j=prev5[j];
        }
        int u=y;
        while(u!=s){
            path1.push_back(prev[u]);
            u=prev[u];
        }
       
         for(int m=1;m<=path1.size();m++){
            path.push_back(path1[path1.size()-m]);
        }
        
        
        
        
        
        
        if(printPath){
    PrintRange(path.begin(), path.end());
    }}









    else if(val5<val4 && val5<=l){
        std::cout<<"YES DORM "<< val5 <<"MINUTES"<<std::endl;
        int i=d;
        path1.push_back(d);
        while(i!=y){
            path1.push_back(prev2[i]);
            i=prev[i];
        }
        int j=y;
        
        while(j!=s){
            path1.push_back(prev[j]);
            j=prev[j];
        }
       
         for(int m=1;m<=path1.size();m++){
            path.push_back(path1[path1.size()-m]);
        }
         if(printPath){
    PrintRange(path.begin(), path.end());}
    }
    else if(val4<=val5 && val4<=l){
        
        std::cout<<"YES PRINTER "<< val4 <<"MINUTES"<<std::endl;
        int i=d;
        path1.push_back(d);
        while(i!=x){
            path1.push_back(prev1[i]);
            i=prev1[i];
        }
        int j=x;
        
        while(j!=s){
            path1.push_back(prev[j]);
            j=prev[j];
        }
       
         for(int m=1;m<=path1.size();m++){
            path.push_back(path1[path1.size()-m]);
        }
   
         if(printPath){
    PrintRange(path.begin(), path.end());}
    }
    else{
        std::cout<<"YES DIRECTLY "<< val3 <<"MINUTES"<<std::endl;
        int i=d;
        path1.push_back(d);
        while(i!=s){
            path1.push_back(prev[i]);
            i=prev[i];
        }
        int t=path.size();
    for(int m=1;m<=path1.size();m++){
            path.push_back(path1[path1.size()-m]);
        }
    if(printPath){
    PrintRange(path.begin(), path.end());}}
    
}

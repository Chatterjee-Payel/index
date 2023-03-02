# index

  public:
    int findExtra(int a[], int b[], int n) {
        // add code here.
        unordered_map<int,int>mp;
        for(int i=0;i<n;i++){
            mp[b[i]]++;
        }
        for(int j=0;j<n;j++){
            if(mp[a[j]]==0){
                return j;
            }
        }
    }
};

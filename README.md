# ML-notes

### 0. **Future of ML:**

![image](https://user-images.githubusercontent.com/54764108/164034377-dc2d63cc-c668-4386-8269-c4fad7b24c1f.png)


### 1. Data Preprocessing: 
from sklearn.preprocessing import Imputer was deprecated with scikit-learn v0.20.4 and removed as of v0.22.2.

    from sklearn.impute import SimpleImputer
    imputer = SimpleImputer(missing_values=np.nan, strategy='mean')
    
    

#### taking care of missing data
    from sklearn.impute import SimpleImputer
    imputer = SimpleImputer(missing_values=np.nan, strategy='mean')
    imputer = imputer.fit(x[:, 1:3])
    x[:, 1:3] = imputer.transform(x[:, 1:3])
  
#### categorical data    
    #columnTransformer
    from sklearn.compose import ColumnTransformer
    columnTransformer = ColumnTransformer([('encoder', OneHotEncoder(), [0])], remainder='passthrough')
    x = np.array(columnTransformer.fit_transform(x),dtype=np.str)

#### splitting test train    
    from sklearn.model_selection import train_test_split
    x_train, x_test, y_train, y_test = train_test_split(x,y, test_size= 0.2, random_state = 0)
    
    
#### feature scaling    
![image](https://user-images.githubusercontent.com/54764108/164050080-6b2d178a-ab0b-48bc-9d69-e780c30b0b22.png)

    from sklearn.preprocessing import StandardScaler
    sc_x = StandardScaler()
    x_train = sc_x.fit_transform(x_train)
    x_test = sc_x.transform(x_train)




 

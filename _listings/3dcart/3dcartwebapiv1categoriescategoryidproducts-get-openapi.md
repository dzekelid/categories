---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Get all products from a specific category
  version: 1.0.0
  description: Get all products from a specific category.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Categories:
    get:
      summary: Get all Categories
      description: Get all categories.
      operationId: Category_GetAllCategories
      x-api-path-slug: 3dcartwebapiv1categories-get
      parameters:
      - in: query
        name: category
        description: Name of the Category
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Categories
    put:
      summary: This method is used to update multiple category records in the database.
        No {categoryid} parameters should be included.
      description: This method is used to update multiple category records in the
        database. no {categoryid} parameters should be included..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categories-put
      parameters:
      - in: body
        name: categories
        description: A Json or XML object containing the new categories
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Category
      - Records
      - In
      - Database
      - ""
      - "No"
      - Categoryid
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new category to the system
      description: Adds a new category to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categories-post
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Category
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Categories:
    get:
      summary: Get the categories from a specific Product
      description: Get the categories from a specific product.
      operationId: Products_GetAllProductCategories
      x-api-path-slug: 3dcartwebapiv1productscatalogidcategories-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Categories
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Categories/{categoryid}:
    put:
      summary: This method is used to update a single category record in the database.
        The {categoryid} parameter specifies which category to update.
      description: This method is used to update a single category record in the database.
        the {categoryid} parameter specifies which category to update..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryid-put
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryid
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Category
      - Record
      - In
      - Database
      - ""
      - Categoryid
      - Parameter
      - Specifies
      - Which
      - Category
      - To
      - Update
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    get:
      summary: Get the options from a specific Category
      description: Get the options from a specific category.
      operationId: Category_GetAllCategoryOptions
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-get
      parameters:
      - in: path
        name: categoryid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Category
    put:
      summary: Updates a collection of options from a specific Category
      description: Updates a collection of options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Category
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-post
      parameters:
      - in: path
        name: categoryid
        description: Category ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Category
      description: Updates specific options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptionsoptionsetid-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{categoryid}/Products:
    get:
      summary: Get all products from a specific category
      description: Get all products from a specific category.
      operationId: Products_GetAllProductsFromCategory
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidproducts-get
      parameters:
      - in: path
        name: categoryid
        description: ID of the category
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{id}:
    get:
      summary: Get a Category
      description: Get a category.
      operationId: Category_GetCategory
      x-api-path-slug: 3dcartwebapiv1categoriesid-get
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Category
    delete:
      summary: Deletes a Category in the system
      description: Deletes a category in the system.
      operationId: Category_Delete
      x-api-path-slug: 3dcartwebapiv1categoriesid-delete
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - In
      - System
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
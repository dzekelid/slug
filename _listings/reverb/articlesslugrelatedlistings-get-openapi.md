---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Articles Slug Related Listings
  description: Find listings related to an article
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /curated_sets/{slug}:
    get:
      summary: Get Curated Sets Slug
      description: Get curated sets slug.
      operationId: getCuratedSetsSlug
      x-api-path-slug: curated-setsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Curated
      - Sets
      - Slug
  /handpicked/{slug}:
    get:
      summary: Get Handpicked Slug
      description: Get results from a handpicked collection
      operationId: getHandpickedSlug
      x-api-path-slug: handpickedslug-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: path
        name: slug
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Handpicked
      - Slug
  /listings/{slug}:
    delete:
      summary: Delete Listings Slug
      description: Delete a draft listing. Cannot be used on non-drafts.
      operationId: deleteListingsSlug
      x-api-path-slug: listingsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    get:
      summary: Get Listings Slug
      description: Get listings slug.
      operationId: getListingsSlug
      x-api-path-slug: listingsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    put:
      summary: Put Listings Slug
      description: Put listings slug.
      operationId: putListingsSlug
      x-api-path-slug: listingsslug-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
  /listings/{slug}/edit:
    get:
      summary: Get Listings Slug Edit
      description: Get listings slug edit.
      operationId: getListingsSlugEdit
      x-api-path-slug: listingsslugedit-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Edit
  /listings/{slug}/flag:
    post:
      summary: Post Listings Slug Flag
      description: Flag a listing for inappropriate content or fraud
      operationId: postListingsSlugFlag
      x-api-path-slug: listingsslugflag-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Flag
  /listings/{slug}/reviews:
    get:
      summary: Get Listings Slug Reviews
      description: Get listings slug reviews.
      operationId: getListingsSlugReviews
      x-api-path-slug: listingsslugreviews-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Reviews
    post:
      summary: Post Listings Slug Reviews
      description: Create a review for a listing
      operationId: postListingsSlugReviews
      x-api-path-slug: listingsslugreviews-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Reviews
  /listings/{slug}/similar_listings:
    get:
      summary: Get Listings Slug Similar Listings
      description: Get listings slug similar listings.
      operationId: getListingsSlugSimilarListings
      x-api-path-slug: listingsslugsimilar-listings-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Similar
      - Listings
  /my/follows/brands/{slug}:
    delete:
      summary: Delete My Follows Brands Slug
      description: Delete my follows brands slug.
      operationId: deleteMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    get:
      summary: Get My Follows Brands Slug
      description: Get my follows brands slug.
      operationId: getMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    post:
      summary: Post My Follows Brands Slug
      description: Post my follows brands slug.
      operationId: postMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
  /my/follows/collections/{slug}:
    delete:
      summary: Delete My Follows Collections Slug
      description: Delete my follows collections slug.
      operationId: deleteMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
    get:
      summary: Get My Follows Collections Slug
      description: Get my follows collections slug.
      operationId: getMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
    post:
      summary: Post My Follows Collections Slug
      description: Post my follows collections slug.
      operationId: postMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
  /my/follows/handpicked/{slug}:
    delete:
      summary: Delete My Follows Handpicked Slug
      description: Delete my follows handpicked slug.
      operationId: deleteMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
    get:
      summary: Get My Follows Handpicked Slug
      description: Follow status for a handpicked collection
      operationId: getMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
    post:
      summary: Post My Follows Handpicked Slug
      description: Post my follows handpicked slug.
      operationId: postMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
  /my/follows/shops/{slug}:
    delete:
      summary: Delete My Follows Shops Slug
      description: Delete my follows shops slug.
      operationId: deleteMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
    get:
      summary: Get My Follows Shops Slug
      description: Get my follows shops slug.
      operationId: getMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
    post:
      summary: Post My Follows Shops Slug
      description: Post my follows shops slug.
      operationId: postMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
  /my/listings/{slug}/state/end:
    put:
      summary: Put My Listings Slug State End
      description: Put my listings slug state end.
      operationId: putMyListingsSlugStateEnd
      x-api-path-slug: mylistingsslugstateend-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
      - Slug
      - State
      - End
  /products/{slug}/reviews:
    get:
      summary: Get Products Slug Reviews
      description: View reviews of a comparison shopping page
      operationId: getProductsSlugReviews
      x-api-path-slug: productsslugreviews-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Products
      - Slug
      - Reviews
    post:
      summary: Post Products Slug Reviews
      description: Create a review for a product
      operationId: postProductsSlugReviews
      x-api-path-slug: productsslugreviews-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Products
      - Slug
      - Reviews
  /sales/{slug}:
    get:
      summary: Get Sales Slug
      description: Get sales slug.
      operationId: getSalesSlug
      x-api-path-slug: salesslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Slug
  /shops/{slug}:
    get:
      summary: Get Shops Slug
      description: Get details on a shop.
      operationId: getShopsSlug
      x-api-path-slug: shopsslug-get
      parameters:
      - in: query
        name: include_listing_count
        description: Include the live listing count in the response
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
  /shops/{slug}/feedback:
    get:
      summary: Get Shops Slug Feedback
      description: Get shops slug feedback.
      operationId: getShopsSlugFeedback
      x-api-path-slug: shopsslugfeedback-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
  /shops/{slug}/feedback/buyer:
    get:
      summary: Get Shops Slug Feedback Buyer
      description: Get seller's feedback as a buyer
      operationId: getShopsSlugFeedbackBuyer
      x-api-path-slug: shopsslugfeedbackbuyer-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
      - Buyer
  /shops/{slug}/feedback/seller:
    get:
      summary: Get Shops Slug Feedback Seller
      description: Get seller's feedback as a seller
      operationId: getShopsSlugFeedbackSeller
      x-api-path-slug: shopsslugfeedbackseller-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
      - Seller
  /articles/{slug}:
    get:
      summary: Get Articles Slug
      description: Display a single article
      operationId: getArticlesSlug
      x-api-path-slug: articlesslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Slug
  /articles/{slug}/related-listings:
    get:
      summary: Get Articles Slug Related Listings
      description: Find listings related to an article
      operationId: getArticlesSlugRelatedListings
      x-api-path-slug: articlesslugrelatedlistings-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Slug
      - Related-listings
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
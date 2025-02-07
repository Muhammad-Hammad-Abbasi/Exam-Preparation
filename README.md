# Next.js Multiple Choice Questions (MCQs)

This document contains multiple-choice questions (MCQs) to test and enhance your knowledge of Next.js. The questions cover the following key topics:

## Topics Covered
1. **Next.js Basics**
2. **Routing in Next.js**
3. **Data Fetching**
   - Server-Side Rendering (SSR) - `getServerSideProps`
   - Static Site Generation (SSG) - `getStaticProps` and `getStaticPaths`
   - Client-Side Fetching - (`useEffect`, SWR)

---

## 1. Next.js Basics

### 1). What command initializes a new Next.js project?
A) `npx create-react-app`
B) `npx create-next-app`
C) `npm create-next-app`
D) `create-next-project`

### 2). Which file in a Next.js project is used to define global configurations?
A) `app.js`
B) `global.config.js`
C) `next.config.js`
D) `server.js`

### 3). What default port does `next dev` use?
A) 3000  
B) 4000  
C) 8080  
D) 8000  

### 4). Which command builds the production-ready files for deployment in Next.js?
A) `npm run dev`  
B) `npm run build`  
C) `npm start`  
D) `next build`  

### 5). What is a key feature of Next.js over React?
A) Static site generation and server-side rendering  
B) Global state management  
C) Improved error boundaries  
D) Built-in React DevTools  

### 6). What file structure does Next.js use to determine routes?
A) `components` directory  
B) `pages` directory  
C) `routes.config.js`  
D) `router.js`  

### 7). How can you configure environment variables in a Next.js project?
A) By creating a `.env.local` file  
B) Through the `next.env.js` file  
C) Using inline definitions in `next.config.js`  
D) Only during runtime  

### 8). What is the role of `_app.tsx` in a Next.js project?
A) To customize server-side logic  
B) To modify the HTML structure of the document  
C) To initialize global settings and providers  
D) To load custom CSS files  

---

## 2. Routing in Next.js

### 9). How do you create dynamic routes in Next.js?
A) By using `[name].tsx` in the `pages` folder  
B) By writing route configurations manually in `routes.js`  
C) Using the `Router` component  
D) Defining URLs inside `next.config.js`  

### 10). What will happen if you navigate to a route not defined in the `pages` folder?
A) A default 404 error page will display  
B) A runtime error will occur  
C) It redirects to `/`  
D) The app crashes  

### 11). What method is used to programmatically navigate in Next.js?
A) `history.push`  
B) `window.location.href`  
C) `useRouter().push()`  
D) `next.navigate()`  

### 12). Can multiple parameters be used in a dynamic route?
A) Yes, by using `[...slug].tsx`  
B) Yes, using multiple query strings  
C) No, only one parameter is allowed  
D) Dynamic routes are limited to static sites  

### 13). How do you define custom headers or meta tags for specific routes?
A) In the `_app.tsx` file  
B) Using the `next-head` module  
C) By adding the `<Head>` component in the page component  
D) By modifying `next.config.js`  

---

## 3. Data Fetching in Next.js

### **Server-Side Rendering (getServerSideProps)**

### 14). When is `getServerSideProps` called?
A) During the build phase  
B) On each request to the server  
C) After the user interacts with the page  
D) Before rendering components on the client-side  

### 15). What must you return from the `getServerSideProps` function?
A) JSON data  
B) Props object inside `{ props: ... }`  
C) An array of data objects  
D) A promise that resolves to HTML  

---

### **Static Site Generation (SSG)**

### 16). What is the purpose of `getStaticProps`?
A) To fetch data during the client-side rendering process  
B) To statically generate pages at build time  
C) To dynamically create server instances  
D) To initialize the app during runtime  

### 17). What additional function is required for dynamic static pages with SSG?
A) `getServerSidePaths`  
B) `getDynamicPaths`  
C) `getStaticPaths`  
D) `getInitialPaths`  

### 18). What does the `fallback` key in `getStaticPaths` control?
A) Whether ungenerated pages return 404  
B) Caching duration  
C) Static resource loading  
D) Incremental server rendering  


## 4).  API Routes and Middleware.

 ### 1). How are API routes defined in a Next.js project?

A) Inside the routes folder
B) Inside the pages/api folder
C) Using routes.js
D) Inside the _api directory

### 2). What is the default HTTP method for an API route in Next.js?

A) GET
B) POST
C) PUT
D) DELETE

### 3). Which Next.js API method is used to handle different HTTP methods in an API route?

A) switch()
B) req.method
C) http.method()
D) route.method

### 4). How do you send a JSON response in a Next.js API route?

A) res.send({})
B) res.end({})
C) res.json({})
D) res.writeJSON({})

### 5). What happens if you create a file named hello.ts in the pages/api directory?

A) The /api/hello endpoint is automatically created
B) A compilation error occurs
C) It creates a route in pages/hello
D) The file is ignored

### 6). What file extension is required for API route files?

A) .json
B) .api
C) .ts or .js
D) .route

### 7). How do you access query parameters in an API route?

A) req.query
B) req.params
C) req.data
D) req.body.query

### 8). What is the purpose of middleware in Next.js?

A) To handle database queries
B) To intercept and modify requests or responses
C) To fetch client-side data
D) To route client requests to third-party services

### 9). Where is middleware configured in a Next.js application?

A) In middleware.ts at the root directory
B) Inside the pages/api/middleware folder
C) Using a routes.middleware.js file
D) Inside next.config.js

### 10). What library is commonly used with middleware for request parsing?

A) express
B) next/body-parser
C) body-parser
D) Middleware does not require any library

### 11). How do you limit API routes to specific HTTP methods in Next.js?

A) Check req.method manually in each route
B) By defining HTTP methods in next.config.js
C) Using a built-in method in Next.js
D) HTTP method limits are not possible

### 12). What will happen if you call an undefined API route in Next.js?

A) The request throws a runtime error
B) A default 404 response is returned
C) The application crashes
D) It redirects to /api/undefined

### 13). How do you add custom headers to a response in an API route?

A) res.setHeader()
B) res.headers()
C) req.setHeader()
D) Custom headers cannot be added

### 14). Can API routes in Next.js be deployed as serverless functions?

A) Yes, all API routes are serverless by default
B) No, they require a dedicated server
C) Only if configured in next.config.js
D) Only for specific providers like AWS

### 15). How do you handle CORS in Next.js API routes?

A) Using cors middleware package
B) Through next.config.js
C) By editing _app.tsx
D) CORS cannot be configured in Next.js

### 16). What key property do you use in the middleware function to modify the request object?

A) req.nextUrl
B) req.update()
C) req.middleware()
D) req.redirectUrl

### 17). What is the NextResponse object used for in middleware?

A) To fetch server data
B) To send custom responses
C) To initialize API routes
D) To define global headers

### 18). How do you enable file uploads in Next.js API routes?

A) Using the multer package
B) By configuring next.fileUpload()
C) API routes cannot handle file uploads
D) Using file-handler middleware

### 19). What is the order of execution when using multiple middlewares?

A) Based on their alphabetical order
B) In the order they are imported or declared
C) Randomized order
D) Determined by Next.js

### 20). Can API routes be authenticated using middleware?

A) Yes, by intercepting the request in the middleware
B) No, authentication must happen in the frontend
C) Only using auth.js in the pages directory
D) Middleware cannot be used for authentication

## 5). Static Site Generation and ISR (20 MCQs).

### 1). What method is used to generate static pages in Next.js?

A) getServerSideProps
B) getStaticProps
C) getInitialProps
D) fetchStaticData

### 2). What is the main purpose of Static Site Generation?

A) To generate pages on every user request
B) To pre-render pages at build time
C) To fetch data client-side
D) To generate pages dynamically

### 3). Which property in getStaticProps determines dynamic routes for SSG?

A) fallback
B) paths
C) dynamicRoutes
D) routePaths

4). What is Incremental Static Regeneration (ISR)?

A) Refreshes all pages after deployment
B) Updates a static page in the background based on user demand
C) Regenerates pages manually by running npm run build
D) An approach used only with dynamic imports

### 5). What Next.js method supports ISR?

A) getServerSideProps
B) getStaticProps with revalidate
C) getStaticPaths
D) useEffect

### 6). In ISR, what does the revalidate field in getStaticProps specify?

A) The number of re-renders for a page
B) The time (in seconds) after which the page regenerates
C) The fallback mode for the page
D) The path for the static file

### 7). What does the fallback: true configuration in getStaticPaths mean?

A) Pages are pre-rendered for all dynamic paths
B) Pages not generated at build time will display a fallback UI while being generated
C) The application shows a 404 page for non-existent paths
D) Static files are not cached

### 8). How is ISR different from traditional SSG?

A) ISR allows updating static content without rebuilding the entire site
B) ISR uses server-side rendering exclusively
C) ISR generates static pages without any data
D) ISR requires manual rebuilding of pages

### 9). What HTTP status code is initially returned for paths in fallback: true?

A) 200
B) 304
C) 404
D) 503

### 10). Which function should you combine with getStaticProps for dynamic SSG paths?

A) getServerSidePaths
B) getStaticPaths
C) useStaticProps
D) fetchStaticRoutes

### 1). In Next.js, what happens when fallback: "blocking" is used?

A) The static page is regenerated after the request is fulfilled
B) Pages not generated at build time will block the request until they are pre-rendered
C) No fallback is allowed, and only pre-defined pages are rendered
D) The page falls back to a server-rendered version permanently

### 12). Which lifecycle does getStaticProps run during?

A) On every user request
B) Only on the client
C) At build time
D) During hydration

### 13). What is a limitation of Static Site Generation?

A) It requires server-side processing
B) Cannot be used for dynamic content
C) Rebuilds are necessary for updates without ISR
D) It does not work with useEffect

### 14). How does ISR enhance static generation?

A) By automatically refreshing cached static pages
B) By allowing a mix of client-side rendering and server-side rendering
C) By offering real-time page updates during runtime
D) By reducing the build time for static files

### 15). What type of content is most suitable for SSG?

A) Content that changes frequently
B) Static content or rarely changing data
C) User-specific data
D) Real-time data

### 16). What environment can ISR pages be updated in without redeploying the entire app?

A) During development only
B) On staging environments
C) On production after deployment
D) Only in localhost

### 17). When using SSG, which build command ensures that all pages are pre-rendered?

A) next dev
B) npm start
C) next build
D) next generate

### 18). Can getStaticProps access cookies or headers?

A) Yes, by using context.req and context.res
B) No, as it runs during build time
C) Only with getStaticPaths
D) Yes, but only in development mode
 
### 19). What is the purpose of the build-id generated in the .next directory?

A) To track ISR updates
B) To ensure static files have unique identifiers
C) To identify the deployed build version
D) To optimize hydration

### 20). What advantage does SSG have over server-side rendering (SSR)?

A) Pages are always up-to-date
B) Reduces server load as pages are pre-built
C) Provides real-time dynamic data
D) Caches data on every user request

---


## 6). Typescript Usage in Next.js (40 MCQs)

- Typing Pages
- API Routes
- Data Fetching
- Custom Types and Utility Functions.

    ###   Typing Pages ( 10 MCQs)

### 1). How can you type props in a functional Next.js page component?

A) props: object
B) props: Props
C) props: React.FC<Props>
D) props: Page<Props>

### 2). What is the correct way to type getStaticProps in TypeScript?

A) export const getStaticProps: StaticPropsType
B) export const getStaticProps: GetStaticProps<Props>
C) export const getStaticProps<Props>
D) export const getStaticProps = (props: Props)

### 3). How do you declare the types for query in getServerSideProps?

A) { query: ParsedUrlQuery }
B) { query: URLSearchParams }
C) { query: Record<string, any> }
D) { query: string }

### 4). How do you type the default export of a page in TypeScript?

A) export default FC<Props>
B) export default React.FC<Props>
C) const Component: FC<Props>
D) export default FunctionComponent<Props>

### 5). Which utility helps in defining typed dynamic routes?

A) DynamicRoutesType
B) NextPage
C) GetRouteTypes
D) InferGetStaticPropsType

### 6). How do you define a Next.js API handler with TypeScript?

A) HandlerType<NextApiRequest>
B) NextApiHandler<Type>
C) ApiRequestHandler
D) RequestHandler<Type>

### 7). What type should be used to type a Head component in Next.js?

A) NextHead
B) JSX.Element
C) ReactNode
D) React.ReactElement

### 8). How do you type static routes with query parameters in a Next.js page?

A) { params: ParsedUrlQuery }
B) { params: StaticPaths }
C) { params: QueryParameters }
D) { params: DynamicProps }

### 9). How do you define the types for router.query in Next.js?

A) query: Record<string, string>
B) query: ParsedUrlQuery
C) query: NextParsedQuery
D) query: GenericQueryParams

### 10). Which Next.js component's props can be typed as NextPage?

A) Head
B) Link
C) Custom Document
D) Page Component

### API Routes ( 10 MCQs)

### 1). What type is used for the req argument in an API route?

A) ApiRequest
B) NextApiRequest
C) RequestProps
D) ApiRouteHandler

### 2). What type should the response (res) argument have in an API route?

A) NextResponseHandler
B) HttpResponse
C) NextApiResponse
D) ApiRouteResponder

### 3). How can you define a custom type for API request body?

A) By using Type<{ body: Props }>.
B) By casting req.body as YourType.
C) Use NextApiBody<Type>.
D) req: Request<Type>

### 4). Which method from NextApiResponse sends a JSON response?

A) res.respond()
B) res.json()
C) res.data()
D) res.sendJson()

### 5). What is the return type of an API route handler?

A) ApiReturnType
B) NextApiResponse<Type>
C) Promise<void>
D) void

### 6). How do you handle CORS in an API route?

A) By modifying NextApiRequest headers
B) Using middleware with cors npm package
C) Configuring .env with CORS rules
D) Adding a response header property

### 7). Can TypeScript enforce API input schema validation in Next.js?

A) Yes, using interfaces only
B) No, you need runtime validators like Zod or Yup
C) Only on SSR
D) Yes, without any runtime validations

### 8). How can you validate request types using Zod in Next.js?

A) By directly attaching Zod to NextApiRequest
B) Parsing req.body through Zod's schema
C) Using Zod middleware
D) It cannot be used

### 9). Which package adds typing for API methods like GET and POST?

A) Next.js API Utilities
B) HTTPMethodEnum from TypeScript-utils
C) NextApiMethods
D) Any TypeScript library like Axios

### 10). What type can strongly type response data sent via res.json()?

A) APIResponseType
B) ApiBody<Type>
C) NextApiResponse<Type>
D) ResponseProps

### Data Fetching (10 MCQs)

### 1). How do you type data returned by getStaticProps?

A) Props
B) StaticPropsData
C) InferGetStaticPropsType<typeof getStaticProps>
D) getStaticType<Props>

### 2). What type represents the return type of getServerSideProps?

A) Promise<{props: Type}>
B) InferSSRReturn<Props>
C) SSRReturnType<Type>
D) GetServerSidePropsContext

### 3). How do you type the return of useSWR in Next.js with TypeScript?

A) const { data } = useSWR<Type>('/api/data')
B) const { data }: SWRResponseType<Type>
C) const { data } = useSWR<{ type: string }>('/api/data')
D) const { data }: SWRHook<Type>

### 4). Which type ensures proper typing for context in getServerSideProps?

A) ServerContextType
B) InferSSRContext<Type>
C) GetServerSidePropsContext
D) SSRContext<Props>

### 5). When typing the result of getStaticPaths, what type is used?

A) StaticPath[]
B) GetStaticPathsResult
C) InferGetStaticPathsType
D) GetStaticPaths<{ id: string }>

### 6). What type should be used to handle dynamic params in getStaticProps?

A) StaticPropsParams<Type>
B) GetStaticPropsContext
C) DynamicPropsHandler
D) PropsContextHandler<Type>

### 7). How can you infer the return type of getStaticProps?

A) GetStaticPropsReturn<typeof getStaticProps>
B) InferGetStaticPropsReturn<Props>
C) InferGetStaticPropsType<typeof getStaticProps>
D) InferPropsReturnType

### 8). What is the default return type for useEffect-based client-side data fetching?

A) Promise<any>
B) void
C) EffectHookReturn
D) AsyncHookResult

### 9). How do you type a SWR mutation function in Next.js?

A) mutate: UseSWRMutateHandler<Type>
B) mutate: SWRMutationHandler<Type>
C) mutate: (data?: Type) => void
D) mutate: HookMutation<Type>

### 10). Can you use TypeScript to enforce return types in getServerSideProps?

A) Yes, always required
B) No, it does not work for server-based data fetching
C) Yes, by defining GetServerSideProps<Type>
D) Not possible in Next.js

## 4. Custom Types and Utility Functions (10 MCQs)

### 1). How can you define a reusable type for an API response in Next.js?

A) type ApiResponse<Type> = { data: Type }
B) export type APIHandler<Type> = { result: Type }
C) Define the type in each API route individually
D) Create a static type for API

### 2). Which TypeScript utility type is helpful for declaring optional props?

A) Optional<T>
B) Partial<T>
C) OptionalsOnly<T>
D) Omit<T>

### 3). How do you create a reusable type for common form inputs?

A) type FormInputs = Record<string, string | number>
B) type FormInputs = Form<string, InputType>
C) Use Inputs<Props> from TS-Lib
D) Define HTMLFormElement inputs manually

### 4). What TypeScript utility allows you to exclude properties from a type?

A) Exclude<T, Properties>
B) Omit<T, Properties>
C) Pick<T, Remaining>
D) FilterProps<T>

### 5). What utility type makes all fields of a type required?

A) MakeRequired<T>
B) Enforce<T>
C) Required<T>
D) Defaultify<T>

### 6). How do you type a custom fetch wrapper utility for JSON responses?

A) type FetchResponse = JSONFetch<Type>
B) const fetch = <T>(): T => ...
C) const fetch: <T>() => Promise<T>
D) function fetchData<T>() {...}

### 7). Which type ensures a utility function receives props from getServerSideProps?

A) NextPageContext
B) InferSSRUtility<Props>
C) GetServerSidePropsType<Props>
D) ContextHandler<Props>

### 8). What generic type ensures correct typing of an array of IDs in dynamic paths?

A) Array<PathTypes>
B) StaticPaths<Array<Type>>
C) PathArrayType<{ id: string }>
D) Array<{ params: { id: string } }>

### 9). How do you enforce type safety for utility functions exporting configs?

A) By using type ConfigUtils<Type>
B) Enforcing export type {...} definitions
C) Declaring TypedConfig<Type>
D) By adding TypeScript interfaces

### 10). What TypeScript utility combines two types into one?

A) Union<Type1, Type2>
B) Merge<Type1, Type2>
C) Intersection<Type1 & Type2>
D) Combine<Type1 | Type2>

---

## 7). Performance Optimization and Best Practices (30 MCQs).

- Code Splitting
- Image Optimization

## Code Splitting (10 MCQs)

### 1). In Next.js, which function can be used to split JavaScript bundles for page-level code splitting?

A) dynamic()
B) useEffect()
C) nextSplit()
D) lazyLoad()

### 2). How can you import a component dynamically without SSR using Next.js?

A) dynamic(() => import('component'), { ssr: false })
B) importLazy('component')
C) dynamic('component', { ssr: true })
D) import('component', { server: false })

### 3). Code splitting improves performance by:

A) Pre-loading all JavaScript at once
B) Only loading required code based on user interaction
C) Using external libraries to load faster
D) Combining large JavaScript files into smaller ones

### 4). Which of the following is the default behavior for React components in Next.js?

A) Synchronous loading
B) Server-side code splitting
C) Automatic code splitting based on routes
D) Asynchronous loading for all components

### 5). To split vendor and application-specific code in a Next.js project, which option do you need?

A) Webpack's splitChunks
B) nextOptimize()
C) lazy(() => component)
D) dynamicPages()

### 6). How do you ensure that a dynamically imported component only loads client-side in Next.js?

A) dynamic(() => import('Component'), { ssr: false })
B) import('Component')
C) lazy(() => import('Component'))
D) Use dynamic imports with default export

### 7). What are the main benefits of implementing code splitting in your Next.js app?

A) Improves developer productivity
B) Reduces initial load time and JavaScript bundle size
C) Increases bundle size
D) Allows immediate reloading

### 8). Which code splitting method ensures chunks are only loaded when a user accesses certain routes?

A) Static Import
B) Import on-demand
C) External scripts
D) Dynamic import with next/dynamic

### 9). Which of the following does dynamic import in Next.js support out of the box?

A) Image files
B) Non-JavaScript files
C) Components with server-side rendering control
D) Third-party CSS files

### 10). Code splitting allows the JavaScript to be sent to the client only for:

A) Components not loaded on-demand
B) Visible sections of the web page
C) Pre-defined user roles
D) All components in the project

### Image Optimization (10 MCQs)

### 1). Which built-in component does Next.js use for image optimization?

A) OptimizedImage 
B) Image
C) LazyImage
D) ResponsiveImage 

### 2). What property in Next.js " Image " component is responsible for serving images in modern formats (like WebP)?

A) layout="responsive"
B) quality
C) format="auto"
D) next-gen="true"

### 3). How can you configure image loading strategy in Next.js?

A) loading="lazy"
B) loading="eager"
C) useResponsiveImages()
D) both eager and lazy

### 4). Which of the following image formats are Next.js capable of serving optimally?

A) JPG
B) WebP
C) AVIF
D) All of the above

### 5). In Next.js, what is the default image format when an image is optimized?

A) PNG
B) JPEG
C) WebP
D) SVG

### 6). To serve images with a responsive layout, which property is typically set in Next.js?

A) layout="intrinsic"
B) layout="responsive"
C) layout="fixed"
D) image="adaptive"

### 7). What does the priority prop do in Next.js "Image" component?

A) Loads the image first, regardless of other resources
B) Defers image loading for background images
C) Defines quality of image served
D) Manages caching options

### 8). Which configuration can help you ensure Next.js serves responsive images across different screen sizes?

A) The sizes attribute in Image 
B) The srcset attribute in Image 
C) Custom Image Optimization in next.config.js
D) Both A and B

### 9). How can Next.js handle images larger than the viewport size?

A) Automatically downscales images
B) Ensures all images are pixel-perfect
C) Favors full-resolution images only
D) Resizes images dynamically based on screen resolution

### 10). What file extensions are supported natively by Next.js for image optimization?

A) PNG, JPEG, and SVG
B) JPEG, WebP, AVIF, PNG
C) JPEG, WebP, MP4
D) PNG, JPEG, GIF

## Bonus - Performance Optimization in Next.js (10 MCQs)

### 1). Which configuration in next.config.js allows custom caching rules for static assets?

A) assetPrefix
B) headers
C) publicRuntimeConfig
D) staticPagePath

### 2). When configuring a custom server in Next.js, what aspect is most important to optimize performance?

A) Adding a third-party service
B) Minifying assets
C) Using server-side rendering only
D) Loading static resources first

### 3). What type of caching strategy can improve repeated visits to your Next.js app?

A) Cache-first strategy
B) Stale-while-revalidate strategy
C) Manual data-fetching for each request
D) Static generation for all pages

### 4). Which method can you use to avoid re-fetching unnecessary data for static pages in Next.js?

A) SSR data hooks
B) Incremental Static Regeneration (ISR)
C) Use getServerSideProps()
D) getInitialProps()

### 5). What effect does the react-helmet package have on performance?

A) It provides dynamic title management
B) Optimizes images through custom tags
C) Works as an automatic bundle loader
D) Provides a global CSS stylesheet

### 6). How do Next.js static pages avoid reloading components with every navigation?

A) By implementing custom revalidation cycles
B) By static HTML rendering
C) By using external JavaScript bundles
D) By SSR (Server-Side Rendering) for all pages

### 7). To improve the initial page load time in Next.js, you should:

A) Use global static data for pages
B) Always use getServerSideProps()
C) Prefetch links and dynamically import non-essential components
D) Manually render every component on the server

### 8). What is the use of next-optimized-images in Next.js?

A) Optimize Next.js app data fetching methods
B) Automate CSS bundling for performance
C) Manage image format and size optimization
D) Control server-side caching for assets

### 9). Which strategy does Next.js use to minimize Javascript overhead when generating pages?

A) On-demand bundling
B) Offload all computations to the backend
C) Client-side rendering exclusively
D) Compression at runtime

### 10). How does Next.js allow you to defer loading critical CSS only when needed?

A) Automatically imports CSS files in client-side JavaScript
B) On-demand CSS loading with next/css
C) Bundles CSS alongside the first page
D) Prioritizes essential CSS before images

---

## 8). Advanced Features (20 MCQs)

## Middleware (10 MCQs)

### 1). In Next.js, middleware allows you to:

A) Create custom routes
B) Manage user authentication globally
C) Fetch data before rendering
D) Perform computations in the background

### 2). Where do you place middleware files in a Next.js project?

A) /pages/middleware
B) /pages/api
C) /middleware
D) /lib

### 3). Which HTTP method is NOT supported in Next.js middleware by default?

A) GET
B) POST
C) PUT
D) PATCH

### 4). Middleware is executed at what stage of the request lifecycle?

A) After data fetching
B) Before routing happens
C) After the page is rendered
D) After the response is sent to the client

### 5). What is one of the primary uses of middleware in Next.js?

A) Dynamic data fetching
B) Error boundary management
C) Modifying requests and responses before they reach the page logic
D) Improving page rendering speed

### 6). Which of the following can be done with middleware in Next.js?

A) Handling redirects and rewrites
B) Altering server-side code
C) Writing inline JSX
D) Fetching dynamic images

### 7). How do you specify which routes the middleware should apply to?

A) By specifying the path inside the middleware file
B) Through the next.config.js file
C) Using the match field in the middleware configuration
D) By defining all routes explicitly in each middleware file

### 8). Which Next.js function is used to terminate middleware early if certain conditions aren't met?

A) res.end()
B) next()
C) return res.redirect()
D) return next()

### 9). Middleware in Next.js operates on which type of response?

A) Client-side only
B) Static HTML responses only
C) All incoming HTTP requests
D) Only dynamically rendered requests

### 10). How can middleware in Next.js impact the performance of an app?

A) Middleware will always slow down the app by introducing delays
B) It won't have any effect on the app’s performance
C) By processing logic before the request reaches pages, it can slow down response times
D) It speeds up the app by processing data after rendering

--- 

## Dynamic Imports (10 MCQs)

### 1). What is the main purpose of using dynamic imports in Next.js?

A) To optimize CSS imports
B) To import modules only when required (on-demand loading)
C) To minimize image sizes
D) To load pages in a fixed order

### 2). Which function does Next.js use to dynamically import a component?

A) dynamic()
B) importAsync()
C) loadComponent()
D) asyncComponent()

### 3). What is a key feature of dynamic() in Next.js when importing components?

A) It supports server-side rendering by default
B) It automatically splits the bundles only when the component is accessed
C) It imports components synchronously
D) It changes the file path dynamically based on user input

### 4). What is the main advantage of dynamically importing a component with SSR disabled ({ ssr: false })?

A) It improves SEO for server-rendered pages
B) It prevents components from being rendered on the server
C) It can only be loaded on the server-side
D) It helps with preloading images faster

### 5). What parameter can be passed into dynamic() to specify a loading indicator while the component loads?

A) loading={true}
B) loading={<div>Loading...</div>}
C) lazy={true}
D) isLoading={true}

### 6). Which of the following is an example of dynamic imports with next/dynamic in Next.js?

A) import('Component')
B) dynamic(() => import('Component'))
C) lazy('Component')
D) dynamic('Component', { ssr: true })

### 7). What will happen if a dynamic component fails to load in Next.js?

A) It will block the entire page from rendering
B) An error will be thrown in the browser console
C) A fallback UI (if provided) will display until the component loads
D) It will silently fail without any impact on the page

### 8). What is one use case for using dynamic imports in Next.js?

A) To dynamically adjust page layouts based on screen size
B) To enable image optimization on client-side only
C) To load large dependencies or components when they're needed, rather than at the start
D) To send components from the server for fast rendering

### 9). When using dynamic imports, the components are treated as:

A) Static components
B) Non-SSR components
C) Separate JavaScript bundles
D) Preact components

### 10). Can dynamic imports improve the performance of large Next.js apps?

A) No, dynamic imports generally make things slower
B) Yes, by reducing the initial JavaScript bundle size
C) No, they’re less optimized than static imports
D) Yes, by ensuring that all resources are loaded on the server first.

---

## 9). Deployment (20 MCQs)

## Vercel (10 MCQs)

### 1). What is Vercel used for in the context of Next.js development?

A) Building static websites
B) Hosting and deploying Next.js applications
C) Designing front-end layouts
D) Debugging JavaScript code

### 2). Which of the following is a feature of Vercel when deploying Next.js apps?

A) Real-time analytics for app usage
B) Auto-scaling and CDN-backed deployment
C) Built-in email management for users
D) Handling back-end databases only

### 3). Which command is typically used to deploy a Next.js application on Vercel?

A) vercel deploy
B) npm deploy
C) next deploy
D) vercel next

### 4). Vercel automatically handles which feature for Next.js apps upon deployment?

A) Database integration
B) Automatic image compression
C) Server-side rendering (SSR)
D) JavaScript bundling

### 5). How does Vercel scale your Next.js application when the traffic increases?

A) It manually updates server settings
B) It uses CDN to serve static assets
C) It auto-scales based on demand
D) It runs on multiple physical servers in parallel

### 6). What is one of the first steps for deploying a Next.js app to Vercel?

A) Connect a GitHub or GitLab repository
B) Edit the next.config.js file
C) Install external libraries for routing
D) Create API routes

### 7). Vercel allows automatic deployment from which version control platforms?

A) GitHub only
B) GitLab only
C) GitHub and GitLab
D) Bitbucket only

### 8). Which of the following will NOT result in a successful deployment on Vercel?

A) Pushing to a connected repository on GitHub
B) Deploying a Next.js app without a package.json file
C) Configuring environmental variables
D) Setting up custom domains

### 9). Can you use Vercel for both front-end and back-end applications in Next.js?

A) No, Vercel is only for static sites
B) Yes, it supports both front-end and API routes
C) Vercel only works for back-end apps
D) No, it's only for deploying static images

### 10). How does Vercel optimize the delivery of static assets for a Next.js application?

A) By compiling all assets to serverless functions
B) By compressing images using third-party services
C) By serving them via its integrated CDN
D) By dynamically serving them from a centralized server

---

## Environment Variables (10 MCQs)

### 1). What is the purpose of environment variables in a Next.js app?

A) To enable routing between pages
B) To manage settings that change based on the environment (e.g., production or development)
C) To import CSS styles
D) To write custom JavaScript code for client-side logic

### 2). Where can you store environment variables for your Next.js app?

A) In the global package.json file
B) In .env.local, .env.development, or .env.production files
C) In a file called config.json
D) In the browser's localStorage

### 3). Which file is intended for storing environment variables that will NOT be committed to version control?

A) .env.local
B) .env.production
C) next.config.js
D) config.env

### 4). To make an environment variable available to the browser, how should it be prefixed?

A) NEXT_PUBLIC_
B) BROWSER_
C) PUBLIC_
D) CLIENT_

### 5). Which environment variable should be used to store a sensitive API key?

A) NEXT_PUBLIC_API_KEY
B) PUBLIC_API_KEY
C) API_KEY
D) .env.production (without a prefix)

### 6). How can environment variables be accessed inside your Next.js application?

A) By using process.env.VARIABLE_NAME
B) By defining them in the next.config.js file
C) Through an API request to an external source
D) By adding them directly in the JSX

### 7). Which of the following should be set in .env.development or .env.local for local development?

A) API endpoint and API keys needed for local testing
B) Port number for the server to run on
C) All production database URLs
D) HTML meta tags

### 8). What happens if you try to use an environment variable that’s not defined in Next.js?

A) The app will crash immediately
B) It will fall back to the default value or undefined
C) It will display a warning in the browser
D) It will automatically create a new environment variable

### 9). Which of the following is NOT an environment variable file supported by Next.js?

A) .env.development.local
B) .env.local
C) .env.config
D) .env.production

### 10). How can you ensure that environment variables work only in production in Next.js?

A) Only define them in .env.local
B) Define them without the NEXT_PUBLIC_ prefix
C) Only define them in .env.production
D) Hardcode them into the code

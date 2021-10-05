# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `NetStorm - Angular 12 NFT Marketplace` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.scss']
})
export class AppComponent {
  title = 'netstorm';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ActivitySectionComponent } from './components/activity-section/activity-section.component';
import { AuctionsOneSectionComponent } from './components/auctions/auctions-one-section/auctions-one-section.component';
import { AuctionsTwoSectionComponent } from './components/auctions/auctions-two-section/auctions-two-section.component';
import { AuctionsThreeSectionComponent } from './components/auctions/auctions-three-section/auctions-three-section.component';
import { AuthorSectionComponent } from './components/author-section/author-section.component';
import { AuthorProfileSectionComponent } from './components/author-profile-section/author-profile-section.component';
import { AuthorsSectionComponent } from './components/authors-section/authors-section.component';
import { CollectionsSectionComponent } from './components/collections-section/collections-section.component';
import { ContactSectionComponent } from './components/contact-section/contact-section.component';
import { CreateSectionComponent } from './components/create-section/create-section.component';
import { ExploreOneSectionComponent } from './components/explore/explore-one-section/explore-one-section.component';
import { ExploreTwoSectionComponent } from './components/explore/explore-two-section/explore-two-section.component';
import { ExploreThreeSectionComponent } from './components/explore/explore-three-section/explore-three-section.component';
import { ExploreFourSectionComponent } from './components/explore/explore-four-section/explore-four-section.component';
import { ExploreFiveSectionComponent } from './components/explore/explore-five-section/explore-five-section.component';
import { ExploreSixSectionComponent } from './components/explore/explore-six-section/explore-six-section.component';
import { FaqSectionComponent } from './components/faq-section/faq-section.component';
import { FooterSectionComponent } from './components/footer-section/footer-section.component';
import { HeaderSectionComponent } from './components/header-section/header-section.component';
import { HelpCenterSectionComponent } from './components/help-center-section/help-center-section.component';
import { HeroSectionComponent } from './components/hero-section/hero-section.component';
import { ItemDetailsSectionComponent } from './components/item-details-section/item-details-section.component';
import { LoginSectionComponent } from './components/login-section/login-section.component';
import { SignupSectionComponent } from './components/signup-section/signup-section.component';
import { ModalSearchComponent } from './components/modal/modal-search/modal-search.component';
import { ModalMenuComponent } from './components/modal/modal-menu/modal-menu.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { TopSellerSectionComponent } from './components/top-seller-section/top-seller-section.component';
import { WalletSectionComponent } from './components/wallet-section/wallet-section.component';
import { WorkSectionComponent } from './components/work-section/work-section.component';
import { BreadcrumbExploreOneComponent } from './components/breadcrumb/breadcrumb-explore-one/breadcrumb-explore-one.component';
import { BreadcrumbExploreTwoComponent } from './components/breadcrumb/breadcrumb-explore-two/breadcrumb-explore-two.component';
import { BreadcrumbExploreThreeComponent } from './components/breadcrumb/breadcrumb-explore-three/breadcrumb-explore-three.component';
import { BreadcrumbExploreFourComponent } from './components/breadcrumb/breadcrumb-explore-four/breadcrumb-explore-four.component';
import { BreadcrumbLiveAuctionsComponent } from './components/breadcrumb/breadcrumb-live-auctions/breadcrumb-live-auctions.component';
import { BreadcrumbItemDetailsComponent } from './components/breadcrumb/breadcrumb-item-details/breadcrumb-item-details.component';
import { BreadcrumbActivityComponent } from './components/breadcrumb/breadcrumb-activity/breadcrumb-activity.component';
import { BreadcrumbAuthorsComponent } from './components/breadcrumb/breadcrumb-authors/breadcrumb-authors.component';
import { BreadcrumbAuthorComponent } from './components/breadcrumb/breadcrumb-author/breadcrumb-author.component';
import { BreadcrumbWalletConnectComponent } from './components/breadcrumb/breadcrumb-wallet-connect/breadcrumb-wallet-connect.component';
import { BreadcrumbCreateComponent } from './components/breadcrumb/breadcrumb-create/breadcrumb-create.component';
import { BreadcrumbLoginComponent } from './components/breadcrumb/breadcrumb-login/breadcrumb-login.component';
import { BreadcrumbSignupComponent } from './components/breadcrumb/breadcrumb-signup/breadcrumb-signup.component';
import { BreadcrumbBlogComponent } from './components/breadcrumb/breadcrumb-blog/breadcrumb-blog.component';
import { BreadcrumbBlogSingleComponent } from './components/breadcrumb/breadcrumb-blog-single/breadcrumb-blog-single.component';
import { BreadcrumbHelpCenterComponent } from './components/breadcrumb/breadcrumb-help-center/breadcrumb-help-center.component';
import { BreadcrumbContactComponent } from './components/breadcrumb/breadcrumb-contact/breadcrumb-contact.component';
import { ExploreOneComponent } from './themes/explore-one/explore-one.component';
import { ExploreTwoComponent } from './themes/explore-two/explore-two.component';
import { ExploreThreeComponent } from './themes/explore-three/explore-three.component';
import { ExploreFourComponent } from './themes/explore-four/explore-four.component';
import { LiveAuctionsComponent } from './themes/live-auctions/live-auctions.component';
import { ItemDetailsComponent } from './themes/item-details/item-details.component';
import { ActivityComponent } from './themes/activity/activity.component';
import { AuthorsComponent } from './themes/authors/authors.component';
import { AuthorComponent } from './themes/author/author.component';
import { WalletConnectComponent } from './themes/wallet-connect/wallet-connect.component';
import { CreateComponent } from './themes/create/create.component';
import { LoginComponent } from './themes/login/login.component';
import { SignupComponent } from './themes/signup/signup.component';
import { ContactComponent } from './themes/contact/contact.component';
import { BlogSectionComponent } from './components/blog-section/blog-section.component';
import { BlogSingleSectionComponent } from './components/blog-single-section/blog-single-section.component';
import { BlogComponent } from './themes/blog/blog.component';
import { BlogSingleComponent } from './themes/blog-single/blog-single.component';
import { HelpCenterComponent } from './themes/help-center/help-center.component';
import { TopSellerTwoSectionComponent } from './components/top-seller-two-section/top-seller-two-section.component';

@NgModule({
  declarations: [
    AppComponent,
    ThemeOneComponent,
    ActivitySectionComponent,
    AuctionsOneSectionComponent,
    AuctionsTwoSectionComponent,
    AuctionsThreeSectionComponent,
    AuthorSectionComponent,
    AuthorProfileSectionComponent,
    AuthorsSectionComponent,
    CollectionsSectionComponent,
    ContactSectionComponent,
    CreateSectionComponent,
    ExploreOneSectionComponent,
    ExploreTwoSectionComponent,
    ExploreThreeSectionComponent,
    ExploreFourSectionComponent,
    ExploreFiveSectionComponent,
    ExploreSixSectionComponent,
    FaqSectionComponent,
    FooterSectionComponent,
    HeaderSectionComponent,
    HelpCenterSectionComponent,
    HeroSectionComponent,
    ItemDetailsSectionComponent,
    LoginSectionComponent,
    SignupSectionComponent,
    ModalSearchComponent,
    ModalMenuComponent,
    ScrollupComponent,
    TopSellerSectionComponent,
    WalletSectionComponent,
    WorkSectionComponent,
    BreadcrumbExploreOneComponent,
    BreadcrumbExploreTwoComponent,
    BreadcrumbExploreThreeComponent,
    BreadcrumbExploreFourComponent,
    BreadcrumbLiveAuctionsComponent,
    BreadcrumbItemDetailsComponent,
    BreadcrumbActivityComponent,
    BreadcrumbAuthorsComponent,
    BreadcrumbAuthorComponent,
    BreadcrumbWalletConnectComponent,
    BreadcrumbCreateComponent,
    BreadcrumbLoginComponent,
    BreadcrumbSignupComponent,
    BreadcrumbBlogComponent,
    BreadcrumbBlogSingleComponent,
    BreadcrumbHelpCenterComponent,
    BreadcrumbContactComponent,
    ExploreOneComponent,
    ExploreTwoComponent,
    ExploreThreeComponent,
    ExploreFourComponent,
    LiveAuctionsComponent,
    ItemDetailsComponent,
    ActivityComponent,
    AuthorsComponent,
    AuthorComponent,
    WalletConnectComponent,
    CreateComponent,
    LoginComponent,
    SignupComponent,
    ContactComponent,
    BlogSectionComponent,
    BlogSingleSectionComponent,
    BlogComponent,
    BlogSingleComponent,
    HelpCenterComponent,
    TopSellerTwoSectionComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- explore-one ( explore demo 1)
    |-- explore-two ( explore demo 2)
    .....
    |-- help-center ( help-center demo )
```

`themes` folder contains the main theme demo.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { RouterModule, Routes } from '@angular/router';

import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ExploreOneComponent } from './themes/explore-one/explore-one.component';
import { ExploreTwoComponent } from './themes/explore-two/explore-two.component';
import { ExploreThreeComponent } from './themes/explore-three/explore-three.component';
import { ExploreFourComponent } from './themes/explore-four/explore-four.component';
import { LiveAuctionsComponent } from './themes/live-auctions/live-auctions.component';
import { ItemDetailsComponent } from './themes/item-details/item-details.component';
import { ActivityComponent } from './themes/activity/activity.component';
import { AuthorsComponent } from './themes/authors/authors.component';
import { AuthorComponent } from './themes/author/author.component';
import { WalletConnectComponent } from './themes/wallet-connect/wallet-connect.component';
import { CreateComponent } from './themes/create/create.component';
import { LoginComponent } from './themes/login/login.component';
import { SignupComponent } from './themes/signup/signup.component';
import { ContactComponent } from './themes/contact/contact.component';
import { BlogComponent } from './themes/blog/blog.component';
import { BlogSingleComponent } from './themes/blog-single/blog-single.component';
import { HelpCenterComponent } from './themes/help-center/help-center.component';

const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'explore-one', component: ExploreOneComponent},
  {path: 'explore-two', component: ExploreTwoComponent},
  {path: 'explore-three', component: ExploreThreeComponent},
  {path: 'explore-four', component: ExploreFourComponent},
  {path: 'auctions', component: LiveAuctionsComponent},
  {path: 'item-details', component: ItemDetailsComponent},
  {path: 'activity', component: ActivityComponent},
  {path: 'authors', component: AuthorsComponent},
  {path: 'author', component: AuthorComponent},
  {path: 'wallet-connect', component: WalletConnectComponent},
  {path: 'create', component: CreateComponent},
  {path: 'login', component: LoginComponent},
  {path: 'signup', component: SignupComponent},
  {path: 'contact', component: ContactComponent},
  {path: 'blog', component: BlogComponent},
  {path: 'blog-single', component: BlogSingleComponent},
  {path: 'help-center', component: HelpCenterComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `hero` , `footer` folder where we wrote our different styled component. For example `hero` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- header-section ( header component folder )
    |-- hero-section ( hero component folder )
    |-- explore ( hero component folder )
        - explore-one-section ( explore section one )
        - explore-two-section ( explore section two )
        ...... ( and other )
    ...    
```

### Contact Page component
`components/contact-section/contact-section.component.html`

```text
|-- components
    ....
    ..
    |-- components ( all components folder )
        ......
        - contact-section ( contact section component )
        ...... ( and other )
    ...    
```

```html
<div class="main">
    <app-header-section></app-header-section>
    <app-breadcrumb-contact></app-breadcrumb-contact>
    <app-contact-section></app-contact-section>
    <app-footer-section></app-footer-section>
    <app-modal-search></app-modal-search>
    <app-modal-menu></app-modal-menu>
    <app-scrollup></app-scrollup>
</div>
```


## theme installtion
To install the theme you have to install [angular](https://angular.io/cli) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build netstorm -c production
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)

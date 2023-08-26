# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/sam7409/NewFAQ#using-the-github-repository) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/sam7409/NewFAQ/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/sam7409/NewFAQ/DataSource/_data/supportdocs_datasource.json</a>

<details markdown="1">
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/aheze/SupportDocs/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/aheze/SupportDocs/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://aheze.github.io/SupportDocs/404) (SupportDocs Integrated File) ([edit](https://github.com/aheze/SupportDocs/edit/DataSource/404.md)) 
- [Neeshu Kumar](https://sam7409.github.io/NewFAQ/Sample-Structure/Profile) (neeshu) ([edit] (https://github.com/sam7409/NewFAQ/edit/DataSource/Sample-Structure/Profile.md)
- [Apple smoothie](https://sam7409.github.io/NewFAQ/Sample-Smoothies/Apple) (smoothies) ([edit](https://github.com/sam7409/NewFAQ/edit/DataSource/Sample-Smoothies/Apple.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/aheze/SupportDocs/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/aheze/SupportDocs/edit/DataSource/_scripts/README.md). 

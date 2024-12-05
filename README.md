This application uses custom response from https://dummyjson.com.
Just incase the API is discarded from dummyjson site, please make below changes


Uncomment first section and comment other code to load the application from mock file.
This commented is added intentionally.

struct BeSocialApp: App {
    var body: some Scene {
        WindowGroup {
//          Uncomment this code if unable to get response from dummyjson site
            FeedView(viewModel: FeedViewModel(networkManager: MockFeedsService()))

//            Uncomment this code if dummyjson site is able to send our mocked response
//            FeedView(viewModel: FeedViewModel(networkManager: FeedsService()))
        }
    }
}

NOTE: Project is added in zip file because I uploaded the application from browser.
I don't have a personal latest Mac which supports xCode for SwiftUI coding.

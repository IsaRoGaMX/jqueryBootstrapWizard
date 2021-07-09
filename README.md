# jqueryBootstrapWizard

jQuery plugin to create Wizard using Bootstrap

## Requirements
- [jQuery 3.1.1](https://code.jquery.com/jquery-3.3.1.min.js)
- [Bootstrap 4.3.1](https://github.com/twbs/bootstrap/releases/download/v4.1.3/bootstrap-4.1.3-dist.zip)

## Button Labels

    $.fn.jqueryBootstrapWizard.labels = {
	    btn_back: 'Back',
	    btn_next: 'Next',
	    btn_finish: 'Finish',
	    btn_cancel: 'Cancel'
    }

## Options
|  | default | description |
|--|--|--|
| cancel_url|null|href value for cancel button (required to show cancel button)
| onBeforeShowTab|null|function to be executed before show tab
| onShownTab|null|function to be executed after show tab
| onFinish|null|onclick event handler to finish button

## Handlers
### onBeforeShowTab

    $('#navWizard').jqueryBootstrapWizard({
	    onBeforeShowTab: function(e) {
		    //e.targetIndex: newly activated tab index
		    //e.relatedTargetIndex: previous active tab
	    }
    });

### onShownTab
    $('#navWizard').jqueryBootstrapWizard({
	    onShownTab: function(e) {
		    //e.targetIndex: newly activated tab index
		    //e.relatedTargetIndex: previous active tab
	    }
    });

### onFinish
    $('#navWizard').jqueryBootstrapWizard({
	    onFinish: function() {
	    }
    });

# win32-hideconsole-perl
Perl 5 module for GUI applications (Tk, Win32::GUI, etc.) to hide that annoying console window that appears at execution time

Brandon Bourret (phatwares@cpan.org)

SYNOPSIS

use Tk;

use Win32::HideConsole;
 
hide_console;
 
my $main_window = MainWindow->new();
 
$main_window->Label(

   -text => 'A GUI app with the console hidden!',
   
   -font => 'arial 14')->pack(-side => 'top');
    
$main_window->MainLoop();

Pollutes the namespace with one function: hide_console

METHODS

hide_console

Place this command near the beginning of your code (right after the "use" directives) to hide the console window.

Version History

1.00 - Initial Release

1.01 - Fixed this POD document

1.02 - More documentation fixes

Permission is granted to use this software under the same terms as Perl itself.

Refer to the Perl Artistic license for details.

Credits

Credit goes to "jdporter" who posted this clever solution on PerlMonks. I just modified it a bit and put it in module form for easy reusability.
